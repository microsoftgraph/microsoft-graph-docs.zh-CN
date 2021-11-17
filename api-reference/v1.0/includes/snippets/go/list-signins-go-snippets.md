---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b4ecca5ea04f6f8888802f4d70c19223cf53164
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029252"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.AuditLogs().SignIns().Get(options)


```