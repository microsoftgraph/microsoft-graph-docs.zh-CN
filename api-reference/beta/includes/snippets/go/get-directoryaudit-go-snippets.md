---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d0821e4e4c8de3efee8a9910c7e3ce92fec66f5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987032"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

directoryAuditId := "directoryAudit-id"
result, err := graphClient.AuditLogs().DirectoryAuditsById(&directoryAuditId).Get(options)


```