---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e31e8b194f5a6b9f75063615ab6b1dac5b330217
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999367"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.AuditLogs().DirectoryAudits().Get(options)


```