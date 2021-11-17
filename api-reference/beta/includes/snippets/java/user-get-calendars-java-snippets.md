---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1c5e57c9ba310c976de3a833bbe8f9553f035946d74643a69ead0b2e95546ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333072"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarCollectionPage calendars = graphClient.me().calendars()
    .buildRequest()
    .get();

```