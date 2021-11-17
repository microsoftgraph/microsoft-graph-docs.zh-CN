---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bc4786ee0c968c3899887a78e1877be301c57e3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976408"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSchemaExtension()
id := "courses"
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
options := &msgraphsdk.SchemaExtensionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.SchemaExtensions().Post(options)


```