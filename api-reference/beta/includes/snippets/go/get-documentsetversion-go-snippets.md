---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdca706ff322097db8f6e685bfb19c9bec1597d4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210282"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
documentSetVersionId := "documentSetVersion-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).DocumentSetVersionsById(&documentSetVersionId).Get(nil)


```