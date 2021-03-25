---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e35df1000ba6f2fe1c9d0886d88522efcd4d333
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208531"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = graphClient.privilegedApproval("{id}")
    .buildRequest()
    .get();

```