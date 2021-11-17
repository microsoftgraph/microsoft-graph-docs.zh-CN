---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcd0cc92102989582bad7a00bc4f1eabd43be625
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993059"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupSettingTemplateId := "groupSettingTemplate-id"
result, err := graphClient.GroupSettingTemplatesById(&groupSettingTemplateId).Get(options)


```