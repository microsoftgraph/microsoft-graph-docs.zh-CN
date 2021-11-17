---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd35f961465ccdec7eb61c8d5d2c1a5588d76a09
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013094"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onenoteSectionId := "onenoteSection-id"
result, err := graphClient.Me().Onenote().SectionsById(&onenoteSectionId).Get(options)


```