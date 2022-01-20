---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3157b305b201ba637d8ee9d30eab6466076bcf3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137618"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Skiptoken: "8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4",
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Messages().Delta()().Get(options)


```