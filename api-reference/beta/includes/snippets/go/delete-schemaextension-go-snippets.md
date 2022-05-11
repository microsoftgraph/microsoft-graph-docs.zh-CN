---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e9a548014d938107abf69cc482cc6ad0f067aae
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329001"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

schemaExtensionId := "schemaExtension-id"
graphClient.SchemaExtensionsById(&schemaExtensionId).Delete()


```