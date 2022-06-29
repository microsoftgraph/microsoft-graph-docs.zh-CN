---
title: 通过 Windows 更新 for Business 部署服务注册更新管理
description: 在更新管理中注册设备，以便可以使用 Windows 更新 for Business 部署服务来管理从Windows 更新发送到该设备的内容。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 1606b9a063a11406366f63ae9d26add8ddded96b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437490"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a>通过 Windows 更新 for Business 部署服务注册更新管理

通过 Windows 更新 for Business 部署服务在更新管理中注册设备时，可以使用部署服务管理从Windows 更新发送到该设备的内容。 可以按更新类别在更新管理中注册设备。

目前，部署服务支持注册管理Windows 10功能更新。 目前，部署服务不需要注册Windows 10质量更新的管理，以部署加速的质量更新。

## <a name="enroll-the-device-in-update-management"></a>在更新管理中注册设备

在特定更新类别的管理中注册设备时，部署服务将成为来自Windows 更新的此类更新的颁发机构。 因此，在使用部署服务将更新分配给[部署](windowsupdates-deployments.md)之前，设备不会从Windows 更新接收该类别的更新。 当服务在管理中注册设备时，设备会自动注册到服务 (即，如果) 尚不存在，则会自动创建 [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) 对象。

### <a name="request"></a>请求

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a>响应

``` http
HTTP/1.1 202 Accepted
```

## <a name="check-the-enrollment-state-of-a-device"></a>检查设备的注册状态

可以通过 [获取设备](/graph/api/windowsupdates-azureaddevice-get)并查看 **azureADDevice** 对象上的注册和 **错误** 属性来检查设备的 **注册** 状态。 在更新管理中成功注册的设备在注册集合中具有 [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) 对象，并且在错误集合中没有任何 [可更新的AssetError](/graph/api/resources/windowsupdates-updatableasseterror) 对象。 服务尝试注册但遇到错误的设备已填充了注册和错误的集合。 服务未收到任何注册请求的设备具有用于注册和错误的空集合。

以下示例演示了在服务管理功能更新时成功注册的设备。

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a>响应
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a>取消注册服务管理或从服务注销 

当从服务管理的给定更新类别中取消注册设备时，该设备不再由部署服务管理，并且可能开始根据其策略配置从Windows 更新接收其他更新。 如果设备分配给定更新类别的任何部署，则不会接收该内容。 设备仍向服务注册，并且仍注册并接收其他更新类别的内容 (（如果适用）) 。

### <a name="request"></a>请求

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a>响应

``` http
HTTP/1.1 202 Accepted
```

可以通过删除设备对象，从服务中完全注销设备。 取消注册设备时，服务会自动取消对所有更新类别的管理，并从每个 [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) 和 [updatableAssetGroup](/graph/api/resources/windowsupdates-updatableassetgroup) 中删除该设备。

### <a name="request"></a>请求

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a>响应
``` http
HTTP/1.1 202 Accepted
```

