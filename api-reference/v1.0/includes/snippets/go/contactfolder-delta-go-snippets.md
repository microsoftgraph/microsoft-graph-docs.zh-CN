---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d8f042a9034bf9974d62c6e33e897c24ae8abdd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137674"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "odata.maxpagesize=2"
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    H: headers,
}
result, err := graphClient.Me().ContactFolders().Delta()().Get(options)


```