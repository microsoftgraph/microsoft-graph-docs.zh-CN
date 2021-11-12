---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 003afccebfe0e69079c26b6c03cfd11f463438312f806994501652ba42e70b21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162018"
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

await client.api('/print/connectors/{printConnectorId}')
    .update(printConnector);

```