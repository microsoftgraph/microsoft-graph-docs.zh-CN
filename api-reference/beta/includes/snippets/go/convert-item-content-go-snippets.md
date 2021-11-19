---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfaabb8e69e1207263e402fbd3f27572b5a36c78
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082359"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ContentRequestBuilderGetQueryParameters{
    Format: "%7Bformat%7D",
}
options := &msgraphsdk.ContentRequestBuilderGetOptions{
    Q: requestParameters,
}
driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Content().Get(options)


```