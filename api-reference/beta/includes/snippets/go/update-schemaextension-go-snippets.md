---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adbfb4ddf1a810f902e075a69aeed15b3402e0ba
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412411"
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
result, err := graphClient.SchemaExtensionsById(&schemaExtensionId).Patch(options)


```