---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d0ffaefc2992c0c3f86db72e34ad8f8c5f7c0d6
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210202"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TermCollectionPage children = graphClient.termStore().sets("{setId}").children()
    .buildRequest()
    .get();

```