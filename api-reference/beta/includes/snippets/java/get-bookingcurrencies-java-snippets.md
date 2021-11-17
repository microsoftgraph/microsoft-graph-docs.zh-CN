---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a855683c5e409d36055d2b1aeb30326cdf648c8d2143ed463b814618c81501c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903126"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCurrencyCollectionPage bookingCurrencies = graphClient.bookingCurrencies()
    .buildRequest()
    .get();

```