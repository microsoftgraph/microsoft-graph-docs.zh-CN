---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ceae07def0fa04eaed70e50c1a931645970b8f797a1eaf1fca4ff0977f7a569
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904017"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthCollectionPage healthOverviews = graphClient.admin().serviceAnnouncement().healthOverviews()
    .buildRequest()
    .get();

```