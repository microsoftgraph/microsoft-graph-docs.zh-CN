---
title: sharedAppleDeviceUser 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 46e0993c69a8ae34a54a654959d8d67a1b7f4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394430"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="0fa3f-103">sharedAppleDeviceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fa3f-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="0fa3f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0fa3f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0fa3f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0fa3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fa3f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fa3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fa3f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fa3f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0fa3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0fa3f-108">Properties</span></span>
|<span data-ttu-id="0fa3f-109">属性</span><span class="sxs-lookup"><span data-stu-id="0fa3f-109">Property</span></span>|<span data-ttu-id="0fa3f-110">类型</span><span class="sxs-lookup"><span data-stu-id="0fa3f-110">Type</span></span>|<span data-ttu-id="0fa3f-111">说明</span><span class="sxs-lookup"><span data-stu-id="0fa3f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa3f-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0fa3f-112">userPrincipalName</span></span>|<span data-ttu-id="0fa3f-113">String</span><span class="sxs-lookup"><span data-stu-id="0fa3f-113">String</span></span>|<span data-ttu-id="0fa3f-114">用户名</span><span class="sxs-lookup"><span data-stu-id="0fa3f-114">User name</span></span>|
|<span data-ttu-id="0fa3f-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="0fa3f-115">dataToSync</span></span>|<span data-ttu-id="0fa3f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fa3f-116">Boolean</span></span>|<span data-ttu-id="0fa3f-117">数据同步</span><span class="sxs-lookup"><span data-stu-id="0fa3f-117">Data to sync</span></span>|
|<span data-ttu-id="0fa3f-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="0fa3f-118">dataQuota</span></span>|<span data-ttu-id="0fa3f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="0fa3f-119">Int64</span></span>|<span data-ttu-id="0fa3f-120">数据配额</span><span class="sxs-lookup"><span data-stu-id="0fa3f-120">Data quota</span></span>|
|<span data-ttu-id="0fa3f-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="0fa3f-121">dataUsed</span></span>|<span data-ttu-id="0fa3f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0fa3f-122">Int64</span></span>|<span data-ttu-id="0fa3f-123">数据配额</span><span class="sxs-lookup"><span data-stu-id="0fa3f-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fa3f-124">关系</span><span class="sxs-lookup"><span data-stu-id="0fa3f-124">Relationships</span></span>
<span data-ttu-id="0fa3f-125">无</span><span class="sxs-lookup"><span data-stu-id="0fa3f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fa3f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fa3f-126">JSON Representation</span></span>
<span data-ttu-id="0fa3f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fa3f-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```




