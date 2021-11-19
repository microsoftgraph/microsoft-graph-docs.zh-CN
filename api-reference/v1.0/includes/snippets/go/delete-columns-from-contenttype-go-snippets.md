---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5434b63d27e5e1c07076f2c306478f82a4f19870
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091228"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
contentTypeId := "contentType-id"
columnDefinitionId := "columnDefinition-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).ColumnsById(&columnDefinitionId).Delete(options)


```