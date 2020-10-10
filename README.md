# qr_reader
Compressed JS for a qr code reader and generator. This code is cross-browser and cross-device compatible. This repo is not human-friendly (or portfolio-friendly), but I did use it to mock a wonky proof of concept a short while ago. The JS is first minified to save space, then it is encoded into base 64 and sideloaded into a COTS application's database. It's stored as a blob, in fact, multiple blobs. At invocation, the blobs are selected from the database, then they are read into a server-side handler and decoded from base 64 back into JS. Finally, it is written as text into a dynamically-generated html page which is then served to the user. 

Trust me, this was the only way.
