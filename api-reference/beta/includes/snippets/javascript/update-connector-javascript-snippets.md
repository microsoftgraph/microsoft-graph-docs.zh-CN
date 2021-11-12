---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99a68179ed7382f6eb015b67e3adf1791a8da74a11235432572f62a7be9bdae5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printConnector = {
  displayName: 'ConnectorName',
  fullyQualifiedDomainName: 'CONNECTOR-MACHINE',
  operatingSystem: 'Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555',
  appVersion: '0.19.7338.23496',
  location: {
    latitude: 1.1,
    longitude: 2.2,
    altitudeInMeters: 3
  }
};

await client.api('/print/connectors/{id}')
    .version('beta')
    .update(printConnector);

```