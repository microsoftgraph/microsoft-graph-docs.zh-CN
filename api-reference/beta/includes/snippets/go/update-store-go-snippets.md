---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 571f9293165489ada60cf2c7ff29fe78eb07bf3f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017365"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewStore()
defaultLanguageTag := "en-US"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
options := &msgraphsdk.TermStoreRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.TermStore().Patch(options)


```