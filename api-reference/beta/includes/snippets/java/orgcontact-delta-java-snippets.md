---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54b4405dee66e7f36ad700dbba35cee948eff9e7bb9cfd833da1721ba897fb0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220625"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContactDeltaCollectionPage delta = graphClient.contacts()
    .delta()
    .buildRequest()
    .get();

```