---
title: 通过 Windows 更新 for Business 部署服务注册更新管理
description: 当设备通过 Windows 更新 for Business 部署服务注册更新管理时，可以使用部署服务管理从 Windows 更新 传递到该设备的内容。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: f1a3946d53792ed3daeb348165bee23d936a7e3b
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509327"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a>通过 Windows 更新 for Business 部署服务注册更新管理

当你通过 Windows 更新 for Business 部署服务在更新管理中注册设备时，可以使用部署服务管理从 Windows 更新传递到该设备的内容。 你可以按更新类别在更新管理中注册设备。

现在，部署服务支持注册管理Windows 10更新。 目前，部署服务不需要注册管理质量Windows 10，以部署快速的质量更新。

## <a name="enroll-the-device-in-update-management"></a>在更新管理中注册设备

当你为某个更新类别注册管理中的设备时，部署服务将成为来自该类别的更新Windows 更新。 因此，设备不会接收来自该类别的更新Windows 更新直到使用部署服务将其分配给部署来部署[更新](windowsupdates-deployments.md)。 设备在服务注册管理时将自动注册到服务 (即 [azureADDevice 对象（如果 azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) 对象) ）。

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

可以通过获取设备并查看 **azureADDevice** 对象的 **注册和错误** 属性来检查设备的注册状态。[](/graph/api/windowsupdates-azureaddevice-get) 在更新管理中成功注册的设备在注册集合中具有 [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) 对象，并且错误集合中没有任何 [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) 对象。 服务尝试注册但遇到错误的设备已填充注册和错误的集合。 服务尚未收到任何注册请求的设备具有注册和错误的空集合。

以下示例显示已成功注册服务功能更新管理的设备。

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

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a>注销服务管理或注销服务 

为给定更新类别注销服务管理的设备时，设备不再由部署服务管理，并且可能会开始根据设备策略配置从 Windows 更新接收其他更新。 如果将设备分配给给定更新类别的任何部署，则它不会接收该内容。 设备仍注册到服务中，并且仍在注册并接收其他更新类别 (（如果适用) ）。

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

可以通过删除设备对象从服务中完全注销设备。 当设备注销时，该服务将自动取消注册所有更新类别的管理，并且从每个 [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) 和 [updatableAssetGroup](/graph/api/resources/windowsupdates-updatableassetgroup) 中删除该设备。

### <a name="request"></a>请求

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a>响应
``` http
HTTP/1.1 202 Accepted
```

