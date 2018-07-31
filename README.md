# DrmTools

## PSSH decoder

buscar pssh en wireshark y hacer "copy as hex string"

luego 
python /home/gmiraval/PycharmProjects/DrmTools/shaka/media/pssh-box.py --from-hex <hex string>

Ejemplo:

python /home/gmiraval/PycharmProjects/DrmTools/shaka/media/pssh-box.py --from-hex 0000006e7073736800000000edef8ba979d64acea3c827dcd51d21ed0000004e080112106d5488581e933450137c8c4901bcfb931a15766572696d61747269786361626c65766973696f6e221d723d766d785f7769646576696e655f417274656172484426733d3935302a025344

y veremos el contendo del pssh:

    PSSH Box v0

    System ID: Widevine edef8ba9-79d6-4ace-a3c8-27dcd51d21ed
  
    PSSH Data (size: 78):
  
    Widevine Data:
    
      Key IDs (1):
      
        6d548858-1e93-3450-137c-8c4901bcfb93
        
      Provider: verimatrixcablevision
      
      Content ID: 723D766D785F7769646576696E655F417274656172484426733D393530
