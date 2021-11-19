---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68ddbb29517adcd0dc0158d114b2ba0d35d536ae
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103737"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.AuditLogs().SignIns().Get(options)


```