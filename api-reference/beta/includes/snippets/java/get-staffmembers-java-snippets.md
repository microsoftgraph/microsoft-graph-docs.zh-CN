---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca5e26a0807d50955b06cd6f3e556134f73ec3fd50b9ce058b6b8182b161e963
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105049"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingStaffMemberCollectionPage staffMembers = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").staffMembers()
    .buildRequest()
    .get();

```