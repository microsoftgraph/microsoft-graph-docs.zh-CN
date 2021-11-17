---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 427bb2bd68774cd3ff44e21b44863b68f33e9052626a6533e4d15c2dfdc13f42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104031"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicyCollectionWithReferencesPage tokenIssuancePolicies = graphClient.applications("{id}").tokenIssuancePolicies()
    .buildRequest()
    .get();

```