---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4193a3627d1b3458b102b6214f5f443c0089b903
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865660"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBookingStaffMemberCollectionPage staffMembers = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").staffMembers()
    .buildRequest()
    .get();

```