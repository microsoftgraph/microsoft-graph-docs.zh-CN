---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfc8e7e3dcb1a7f41be889c6325e32a3c3e93b34
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992563"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printServiceId := "printService-id"
result, err := graphClient.Print().ServicesById(&printServiceId).Endpoints().Get(options)


```