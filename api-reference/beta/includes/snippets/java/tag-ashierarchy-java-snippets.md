---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cc8e94b49b92761dba783487ae8f8c463ab2e0a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TagAsHierarchyCollectionPage asHierarchy = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags()
    .asHierarchy()
    .buildRequest()
    .get();

```