---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8fa69be171b42b4206b8de4b62cdd0851504c5d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966540"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

OrgContactDeltaCollectionPage delta = graphClient.contacts()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mail")
    .get();

```