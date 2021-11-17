---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30752701872b092134ea2593cad9cee507cadaf76bb6aa112d0422e18094b5f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333433"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TermCollectionPage children = graphClient.termStore().sets("{setId}").children()
    .buildRequest()
    .get();

```