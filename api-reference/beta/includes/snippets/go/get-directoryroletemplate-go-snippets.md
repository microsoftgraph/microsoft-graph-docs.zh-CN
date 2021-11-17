---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e768239a59b5f2204449a1f6878efdc911d610f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982139"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

directoryRoleTemplateId := "directoryRoleTemplate-id"
result, err := graphClient.DirectoryRoleTemplatesById(&directoryRoleTemplateId).Get(options)


```