# FusionPBX-Advanced-CID-Prefix
How to create caller ID rewriting with regex in FusionPBX

Edit Outbound Route:
effective_caller_id_number=${regex(${outbound_caller_id_number}|^0(.*)$|44%1)}"

Strips 0, any number, concat 44 and concat the rest of the originally called number

