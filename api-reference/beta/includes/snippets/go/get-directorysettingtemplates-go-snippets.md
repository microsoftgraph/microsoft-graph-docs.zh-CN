---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8073811db8bdd7762f4a13e12c7ba2f67333f2fb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092197"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DirectorySettingTemplates().Get(options)


```