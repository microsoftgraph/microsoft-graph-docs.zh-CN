---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75fd85052811b0286c42a13d74f72e688fb2594f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097685"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directorySettingTemplateId := "directorySettingTemplate-id"
result, err := graphClient.DirectorySettingTemplatesById(&directorySettingTemplateId).Get(options)


```