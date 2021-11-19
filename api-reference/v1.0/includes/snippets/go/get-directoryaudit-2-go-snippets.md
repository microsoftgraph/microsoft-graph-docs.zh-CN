---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10b97d0f38446be069c643a221f92721c8209864
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087950"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.AuditLogs().DirectoryAudits().Get(options)


```