---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ca3656efdd68ec4147071a8815e23958719e010
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952423"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource userSource = new UserSource();
userSource.email = "adelev@contoso.com";
userSource.includedSources = EnumSet.of(SourceType.MAILBOX);

graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("387566cc-38ae-4e85-ab4b-cd2dd34faa07").userSources()
    .buildRequest()
    .post(userSource);

```