---
title: sharedAppleDeviceUser 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4dc78ad66302d4ffd330936cc95bd9b3cd7ae900
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383048"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="ae681-103">sharedAppleDeviceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae681-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="ae681-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae681-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae681-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae681-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae681-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae681-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae681-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ae681-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ae681-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae681-108">Properties</span></span>
|<span data-ttu-id="ae681-109">属性</span><span class="sxs-lookup"><span data-stu-id="ae681-109">Property</span></span>|<span data-ttu-id="ae681-110">类型</span><span class="sxs-lookup"><span data-stu-id="ae681-110">Type</span></span>|<span data-ttu-id="ae681-111">说明</span><span class="sxs-lookup"><span data-stu-id="ae681-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae681-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae681-112">userPrincipalName</span></span>|<span data-ttu-id="ae681-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ae681-113">String</span></span>|<span data-ttu-id="ae681-114">用户名</span><span class="sxs-lookup"><span data-stu-id="ae681-114">User name</span></span>|
|<span data-ttu-id="ae681-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="ae681-115">dataToSync</span></span>|<span data-ttu-id="ae681-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae681-116">Boolean</span></span>|<span data-ttu-id="ae681-117">要同步的数据</span><span class="sxs-lookup"><span data-stu-id="ae681-117">Data to sync</span></span>|
|<span data-ttu-id="ae681-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="ae681-118">dataQuota</span></span>|<span data-ttu-id="ae681-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ae681-119">Int64</span></span>|<span data-ttu-id="ae681-120">数据配额</span><span class="sxs-lookup"><span data-stu-id="ae681-120">Data quota</span></span>|
|<span data-ttu-id="ae681-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="ae681-121">dataUsed</span></span>|<span data-ttu-id="ae681-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ae681-122">Int64</span></span>|<span data-ttu-id="ae681-123">数据配额</span><span class="sxs-lookup"><span data-stu-id="ae681-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae681-124">关系</span><span class="sxs-lookup"><span data-stu-id="ae681-124">Relationships</span></span>
<span data-ttu-id="ae681-125">无</span><span class="sxs-lookup"><span data-stu-id="ae681-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae681-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae681-126">JSON Representation</span></span>
<span data-ttu-id="ae681-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae681-127">Here is a JSON representation of the resource.</span></span>
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



