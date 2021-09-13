---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9fa4a71a158a2e5df084eaaf967821216b03746430ca2b823584981b4e60c10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279396"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationDeltaCollectionPage delta = graphClient.applications()
    .delta()
    .buildRequest()
    .get();

```