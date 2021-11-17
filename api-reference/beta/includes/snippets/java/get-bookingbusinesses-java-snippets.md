---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 478e207eadb4a80b8ec7c8a031ebfff0c8a893841e70dbe416ee26acb07c80db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105048"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusinessCollectionPage bookingBusinesses = graphClient.bookingBusinesses()
    .buildRequest()
    .get();

```