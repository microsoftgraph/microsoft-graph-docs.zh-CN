---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1353bca4410c0398a4759af576de69d0b4e63aa625cb4d0d51425ac47bbaa4e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278900"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteCollectionWithReferencesPage followedSites = graphClient.me().followedSites()
    .buildRequest()
    .get();

```