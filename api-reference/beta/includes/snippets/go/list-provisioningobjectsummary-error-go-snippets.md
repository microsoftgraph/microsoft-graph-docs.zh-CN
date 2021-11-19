---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cf8dc8336d7adb07694491c1fab24e6ddac9782
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094009"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.AuditLogs().Provisioning().Get(options)


```