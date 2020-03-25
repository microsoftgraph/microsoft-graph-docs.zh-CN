---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3643bc59c7302aa1a46189c6fe8d9d894a2337bb
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printConnector = {
  name: "ConnectorName",
  fullyQualifiedDomainName: "CONNECTOR-MACHINE",
  operatingSystem: "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  appVersion: "0.19.7338.23496",
  location: {
    latitude: 1.1,
    longitude: 2.2,
    altitudeInMeters: 3
  }
};

let res = await client.api('/print/connectors/{id}')
    .version('beta')
    .update(printConnector);

```