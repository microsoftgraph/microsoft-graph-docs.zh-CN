---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 098072da92a2e8d427027404e9a389e960fb5afd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943687"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AgreementAcceptanceCollectionWithReferencesPage agreementAcceptances = graphClient.me().agreementAcceptances()
    .buildRequest()
    .get();

```