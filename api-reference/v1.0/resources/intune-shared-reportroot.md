---
title: reportRoot 资源类型
description: 表示一个历史记录报告实例的资源。
author: tfitzmac
ms.openlocfilehash: 46b4844487a1cb714dde791e6867c277c1693f66
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303967"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="62a7f-103">reportRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="62a7f-103">reportRoot resource type</span></span>

> <span data-ttu-id="62a7f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="62a7f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62a7f-105">表示一个历史记录报告实例的资源。</span><span class="sxs-lookup"><span data-stu-id="62a7f-105">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="62a7f-106">方法</span><span class="sxs-lookup"><span data-stu-id="62a7f-106">Methods</span></span>
|<span data-ttu-id="62a7f-107">方法</span><span class="sxs-lookup"><span data-stu-id="62a7f-107">Method</span></span>|<span data-ttu-id="62a7f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="62a7f-108">Return Type</span></span>|<span data-ttu-id="62a7f-109">说明</span><span class="sxs-lookup"><span data-stu-id="62a7f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62a7f-110">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="62a7f-110">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|[<span data-ttu-id="62a7f-111">reportRoot</span><span class="sxs-lookup"><span data-stu-id="62a7f-111">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="62a7f-112">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62a7f-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="62a7f-113">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="62a7f-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|[<span data-ttu-id="62a7f-114">reportRoot</span><span class="sxs-lookup"><span data-stu-id="62a7f-114">reportRoot</span></span>](../resources/intune-shared-reportroot.md)|<span data-ttu-id="62a7f-115">更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="62a7f-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="62a7f-116">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="62a7f-116">**Device configuration**</span></span>|
|[<span data-ttu-id="62a7f-117">deviceConfigurationDeviceActivity 函数</span><span class="sxs-lookup"><span data-stu-id="62a7f-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="62a7f-118">报告</span><span class="sxs-lookup"><span data-stu-id="62a7f-118">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="62a7f-119">设备配置设备活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="62a7f-119">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="62a7f-120">deviceConfigurationUserActivity 函数</span><span class="sxs-lookup"><span data-stu-id="62a7f-120">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[<span data-ttu-id="62a7f-121">报告</span><span class="sxs-lookup"><span data-stu-id="62a7f-121">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="62a7f-122">设备配置用户活动报告的元数据</span><span class="sxs-lookup"><span data-stu-id="62a7f-122">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="62a7f-123">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="62a7f-123">**Troubleshooting**</span></span>|
|[<span data-ttu-id="62a7f-124">managedDeviceEnrollmentFailureDetails 函数</span><span class="sxs-lookup"><span data-stu-id="62a7f-124">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="62a7f-125">报告</span><span class="sxs-lookup"><span data-stu-id="62a7f-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="62a7f-126">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="62a7f-126">Not yet documented.</span></span>|
|[<span data-ttu-id="62a7f-127">managedDeviceEnrollmentTopFailures 函数</span><span class="sxs-lookup"><span data-stu-id="62a7f-127">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="62a7f-128">报告</span><span class="sxs-lookup"><span data-stu-id="62a7f-128">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="62a7f-129">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="62a7f-129">Not yet documented.</span></span>|


## <a name="properties"></a><span data-ttu-id="62a7f-130">属性</span><span class="sxs-lookup"><span data-stu-id="62a7f-130">Properties</span></span>
|<span data-ttu-id="62a7f-131">属性</span><span class="sxs-lookup"><span data-stu-id="62a7f-131">Property</span></span>|<span data-ttu-id="62a7f-132">类型</span><span class="sxs-lookup"><span data-stu-id="62a7f-132">Type</span></span>|<span data-ttu-id="62a7f-133">说明</span><span class="sxs-lookup"><span data-stu-id="62a7f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a7f-134">id</span><span class="sxs-lookup"><span data-stu-id="62a7f-134">id</span></span>|<span data-ttu-id="62a7f-135">String</span><span class="sxs-lookup"><span data-stu-id="62a7f-135">String</span></span>|<span data-ttu-id="62a7f-136">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="62a7f-136">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62a7f-137">关系</span><span class="sxs-lookup"><span data-stu-id="62a7f-137">Relationships</span></span>
<span data-ttu-id="62a7f-138">无</span><span class="sxs-lookup"><span data-stu-id="62a7f-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62a7f-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62a7f-139">JSON Representation</span></span>
<span data-ttu-id="62a7f-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62a7f-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a><span data-ttu-id="62a7f-141">示例</span><span class="sxs-lookup"><span data-stu-id="62a7f-141">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```