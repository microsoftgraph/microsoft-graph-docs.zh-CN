---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 488b35e6690d786f6ca0e387ec5fdc3ee630af44
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSchemaExtension()
owner := "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa"
requestBody.SetOwner(&owner)
requestBody.SetProperties( []ExtensionSchemaProperty {
    msgraphsdk.NewExtensionSchemaProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "courseId",
        "type": "Integer",
    }
    msgraphsdk.NewExtensionSchemaProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "courseName",
        "type": "String",
    }
    msgraphsdk.NewExtensionSchemaProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "courseType",
        "type": "String",
    }
    msgraphsdk.NewExtensionSchemaProperty(),
    SetAdditionalData(map[string]interface{}{
        "name": "courseSupervisors",
        "type": "String",
    }
}
options := &msgraphsdk.SchemaExtensionRequestBuilderPatchOptions{
    Body: requestBody,
}
schemaExtensionId := "schemaExtension-id"
graphClient.SchemaExtensionsById(&schemaExtensionId).Patch(options)


```