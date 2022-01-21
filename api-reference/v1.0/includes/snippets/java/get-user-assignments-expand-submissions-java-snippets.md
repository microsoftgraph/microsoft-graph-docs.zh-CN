---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6659b70242654ac9ad670edfbf71d213dbe912e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111069"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "submissions"));

EducationAssignmentCollectionPage assignments = graphClient.education().users("80cefd93-8d88-40e2-b5d3-67898383e226").assignments()
    .buildRequest( requestOptions )
    .get();

```