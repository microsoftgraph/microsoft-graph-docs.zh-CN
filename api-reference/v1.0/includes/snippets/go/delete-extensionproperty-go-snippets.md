---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02eefe4ec1c0e69dbf2ba42a0110e4d46299978e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089026"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
extensionPropertyId := "extensionProperty-id"
graphClient.ApplicationsById(&applicationId).ExtensionPropertiesById(&extensionPropertyId).Delete(options)


```