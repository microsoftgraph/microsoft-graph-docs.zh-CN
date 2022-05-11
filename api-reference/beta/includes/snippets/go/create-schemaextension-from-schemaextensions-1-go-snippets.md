---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fb9ea8cbefdb40a00c3c16df20a60ee205501ae
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327622"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSchemaExtension()
id := "graphlearn_courses"
requestBody.SetId(&id)
description := "Graph Learn training courses extensions"
requestBody.SetDescription(&description)
requestBody.SetTargetTypes( []String {
    "Group",
}
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
}
result, err := graphClient.SchemaExtensions().Post(requestBody)


```