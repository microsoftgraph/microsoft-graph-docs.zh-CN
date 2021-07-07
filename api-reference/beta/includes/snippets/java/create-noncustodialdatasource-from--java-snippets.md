---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f014f894c4e5af06c73cc85801e9be7f5b82a95
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53319498"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSource noncustodialDataSource = new NoncustodialDataSource();
noncustodialDataSource.additionalDataManager().put("@odata.id", new JsonPrimitive("https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"));

graphClient.compliance().ediscovery().cases("06d52284-ed81-49b8-904a-b863d3164731").sourceCollections("12aab1671c834213a84ba219c06f4c5a").noncustodialSources().references()
    .buildRequest()
    .post(noncustodialDataSource);

```