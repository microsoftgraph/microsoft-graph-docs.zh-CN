---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2912fd245624169f4ca9c3745be1e4047b983466cc5ce3dbc290005e6af37547
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219453"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource userSource = new UserSource();
userSource.email = "adelev@contoso.com";
userSource.includedSources = EnumSet.of(SourceType.MAILBOX);

graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("387566cc-38ae-4e85-ab4b-cd2dd34faa07").userSources()
    .buildRequest()
    .post(userSource);

```