---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd0ea6726ab9ab038eff623db42de5cea0ddef89
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995523"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationId := "application-id"
extensionPropertyId := "extensionProperty-id"
graphClient.ApplicationsById(&applicationId).ExtensionPropertiesById(&extensionPropertyId).Delete(options)


```