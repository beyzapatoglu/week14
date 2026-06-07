# week14
def is_bst(self):
    return self.validate(self.root, None, None)

def validate(self, node, minimum, maximum):
    if node == None:
        return True

   if minimum != None and node.data <= minimum:
        return False

  if maximum != None and node.data >= maximum:
        return False

  return self.validate(node.left, minimum, node.data) and \
           self.validate(node.right, node.da
