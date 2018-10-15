# PcmToPM3 Pcm音频转换mp3音频(lame库)



```
NSString *uuid = [[NSUUID UUID] UUIDString];
NSString *pcmPath = [NSString stringWithFormat:@"%@%@.pcm",NSTemporaryDirectory(),uuid];
NSString *mp3Path = [NSString stringWithFormat:@"%@%@.mp3",NSTemporaryDirectory(),uuid];

pcmTomp3 *convert = [[pcmTomp3 alloc] init];
[convert setPcmFilePath:pcmPath];
[convert setMp3FilePath:mp3Path];

if([convert convertToMp3]){
	NSLog(@"转换成功！！");
}

```