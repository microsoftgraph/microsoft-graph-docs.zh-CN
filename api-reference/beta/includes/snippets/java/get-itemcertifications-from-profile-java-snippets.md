---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95cfdb6fa8ea72f4e96c41ba9f7743518dfa16c9ab5f8719f047e057d77cb726
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218995"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCertificationCollectionPage certifications = graphClient.me().profile().certifications()
    .buildRequest()
    .get();

```