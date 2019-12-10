---
title: 列出 androidManagedStoreAppConfigurationSchemas
description: 列出 androidManagedStoreAppConfigurationSchema 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 141c14087405b8c3c009a7fc3d245f2b7db8ca1b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39922711"
---
# <a name="list-androidmanagedstoreappconfigurationschemas"></a><span data-ttu-id="90cad-103">列出 androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="90cad-103">List androidManagedStoreAppConfigurationSchemas</span></span>

> <span data-ttu-id="90cad-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90cad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90cad-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90cad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90cad-106">列出[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90cad-106">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90cad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="90cad-107">Prerequisites</span></span>
<span data-ttu-id="90cad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90cad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90cad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="90cad-110">Permission type</span></span>|<span data-ttu-id="90cad-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90cad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90cad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90cad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90cad-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90cad-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90cad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90cad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90cad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90cad-115">Not supported.</span></span>|
|<span data-ttu-id="90cad-116">Application</span><span class="sxs-lookup"><span data-stu-id="90cad-116">Application</span></span>|<span data-ttu-id="90cad-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90cad-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90cad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90cad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="90cad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="90cad-119">Request headers</span></span>
|<span data-ttu-id="90cad-120">标头</span><span class="sxs-lookup"><span data-stu-id="90cad-120">Header</span></span>|<span data-ttu-id="90cad-121">值</span><span class="sxs-lookup"><span data-stu-id="90cad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90cad-122">授权</span><span class="sxs-lookup"><span data-stu-id="90cad-122">Authorization</span></span>|<span data-ttu-id="90cad-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90cad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90cad-124">接受</span><span class="sxs-lookup"><span data-stu-id="90cad-124">Accept</span></span>|<span data-ttu-id="90cad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90cad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90cad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90cad-126">Request body</span></span>
<span data-ttu-id="90cad-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90cad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90cad-128">响应</span><span class="sxs-lookup"><span data-stu-id="90cad-128">Response</span></span>
<span data-ttu-id="90cad-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="90cad-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90cad-130">示例</span><span class="sxs-lookup"><span data-stu-id="90cad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90cad-131">请求</span><span class="sxs-lookup"><span data-stu-id="90cad-131">Request</span></span>
<span data-ttu-id="90cad-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90cad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="90cad-133">响应</span><span class="sxs-lookup"><span data-stu-id="90cad-133">Response</span></span>
<span data-ttu-id="90cad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90cad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1871

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
      "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
          "index": 5,
          "parentIndex": 11,
          "schemaItemKey": "Schema Item Key value",
          "displayName": "Display Name value",
          "description": "Description value",
          "defaultBoolValue": true,
          "defaultIntValue": 15,
          "defaultStringValue": "Default String Value value",
          "defaultStringArrayValue": [
            "Default String Array Value value"
          ],
          "dataType": "integer",
          "selections": [
            {
              "@odata.type": "microsoft.graph.keyValuePair",
              "name": "Name value",
              "value": "Value value"
            }
          ]
        }
      ],
      "nestedSchemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
          "index": 5,
          "parentIndex": 11,
          "schemaItemKey": "Schema Item Key value",
          "displayName": "Display Name value",
          "description": "Description value",
          "defaultBoolValue": true,
          "defaultIntValue": 15,
          "defaultStringValue": "Default String Value value",
          "defaultStringArrayValue": [
            "Default String Array Value value"
          ],
          "dataType": "integer",
          "selections": [
            {
              "@odata.type": "microsoft.graph.keyValuePair",
              "name": "Name value",
              "value": "Value value"
            }
          ]
        }
      ]
    }
  ]
}
```





