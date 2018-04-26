# -0-python-
一段词查词频并写入字典
#plan A
word = 'As I explained in my temporary certification of October 26, 2017, the American people expect their Government to provide as much access as possible to the President John F. Kennedy Assassination Records (records) so that they may — as they deserve — finally be fully informed about all aspects of this pivotal event.  Over the past 180 days, executive departments and agencies (agencies) have reviewed all of the information within records temporarily withheld from release and have proposed to the Archivist of the United States (Archivist) that certain information should continue to be redacted because of identifiable national security, law enforcement, and foreign affairs concerns.'
keywords= ['I','the']

freqs = []
for keyword in keywords:
    freq = word.split().count(keyword)
    print(freq)
    freqs.append(str(freq))
print(freqs)
# 写入字典
dict(zip(keyword,freqs))   

