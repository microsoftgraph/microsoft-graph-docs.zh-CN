---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddb174ae06ca00da61f002d7fe4207438954d27c56658047de3be5f2b23041b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162460"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionWithReferencesPage allowedGroups = graphClient.print().shares("{id}").allowedGroups()
    .buildRequest()
    .get();

```