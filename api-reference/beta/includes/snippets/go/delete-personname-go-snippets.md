---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 325bfb9dd92e958d95b2630eb6a0b8ec0a8ae97c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Delete(options)


```