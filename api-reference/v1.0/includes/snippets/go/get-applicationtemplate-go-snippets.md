---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d8086bf88563f63900dce69b946ff2eea68ced1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationTemplateId := "applicationTemplate-id"
result, err := graphClient.ApplicationTemplatesById(&applicationTemplateId).Get(options)


```