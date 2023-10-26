# Useful-Code
How to set window for CT images in Slicer:
```
>>> all_nodes = slicer.mrmlScene.GetNodesByClass('vtkMRMLScalarVolumeNode')
>>> for ct in all_nodes:
...     ct.GetDisplayNode().SetAutoWindowLevel(False)
...     ct.GetDisplayNode().SetWindowLevel(1400,-500)
...
>>>
```
