---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 405d4bbcf2ab7cff521da138a71e5e8a8ee226e4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102265"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryRoleTemplateId := "directoryRoleTemplate-id"
result, err := graphClient.DirectoryRoleTemplatesById(&directoryRoleTemplateId).Get(options)


```