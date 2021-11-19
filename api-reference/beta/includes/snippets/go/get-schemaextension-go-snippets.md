---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a863414990bdf2bcdb39235c0e3188f439385bc3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097950"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

schemaExtensionId := "schemaExtension-id"
result, err := graphClient.SchemaExtensionsById(&schemaExtensionId).Get(options)


```