---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73f94b448dabda21daacf134edeb53d658cb298c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999257"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

directoryRoleId := "directoryRole-id"
result, err := graphClient.DirectoryRolesById(&directoryRoleId).Get(options)


```