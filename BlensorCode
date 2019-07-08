import bpy
import math
from bpy import data as D
from bpy import context as C
from mathutils import *
from math import *
import blensor

    
scanner = bpy.data.objects["Camera"]

"""Move it to a different location"""
scanner.location = (0,-10,2)
scanner.rotation_euler= (90/180*pi,0,0)
scanner.scan_type = "tof"

print("\n\n\n\n\n\n")

for item in bpy.data.objects:
    if item.type == 'MESH' and item.name.startswith('Scan'):
        bpy.data.objects.remove(item)
bpy.data.objects["Satellite"].rotation_euler=(60/180*pi,0,0)
bpy.ops.blensor.delete_scans();
bpy.ops.blensor.scan();


f=open("C:/Users/Justice/Desktop/111/test0.txt","w")
for item in bpy.data.objects:
    if item.type == 'MESH' and item.name.startswith('Scan'):
        # Scannerpunkte durchgehen
        for sp in item.data.vertices:
            print('X=%+#5.3f\tY=%+#5.3f\tZ=%+#5.3f' % (sp.co[0], sp.co[1],sp.co[2]))
            str='%#5.3f\t%#5.3f\t%#5.3f \n' % (sp.co[0], sp.co[1],sp.co[2])
            f.write(str)
        print("1 OK")
           
           
           
           
           
for item in bpy.data.objects:
    if item.type == 'MESH' and item.name.startswith('Scan'):
        bpy.data.objects.remove(item)
                
bpy.data.objects["Satellite"].rotation_euler=(0,90/180*pi,0)       
bpy.ops.blensor.delete_scans();
bpy.ops.blensor.scan();            

f=open("C:/Users/Justice/Desktop/111/test1.txt","w")
for item in bpy.data.objects:
    if item.type == 'MESH' and item.name.startswith('Scan'):
        # Scannerpunkte durchgehen
        for sp in item.data.vertices:
            print('X=%+#5.3f\tY=%+#5.3f\tZ=%+#5.3f' % (sp.co[0], sp.co[1],sp.co[2]))
            str='%#5.3f\t%#5.3f\t%#5.3f \n' % (sp.co[0], sp.co[1],sp.co[2])
            f.write(str)
            print("2 OK")
            
            
