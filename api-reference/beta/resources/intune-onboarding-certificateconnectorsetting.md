---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe154ed3150ae434f8068bc04a56dd6e5b48744
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573058"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="d07db-103">certificateConnectorSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="d07db-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="d07db-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d07db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d07db-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d07db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d07db-106">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="d07db-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="d07db-107">属性</span><span class="sxs-lookup"><span data-stu-id="d07db-107">Properties</span></span>
|<span data-ttu-id="d07db-108">属性</span><span class="sxs-lookup"><span data-stu-id="d07db-108">Property</span></span>|<span data-ttu-id="d07db-109">类型</span><span class="sxs-lookup"><span data-stu-id="d07db-109">Type</span></span>|<span data-ttu-id="d07db-110">说明</span><span class="sxs-lookup"><span data-stu-id="d07db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d07db-111">状态</span><span class="sxs-lookup"><span data-stu-id="d07db-111">status</span></span>|<span data-ttu-id="d07db-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d07db-112">Int32</span></span>|<span data-ttu-id="d07db-113">证书连接器状态</span><span class="sxs-lookup"><span data-stu-id="d07db-113">Certificate connector status</span></span>|
|<span data-ttu-id="d07db-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="d07db-114">certExpiryTime</span></span>|<span data-ttu-id="d07db-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d07db-115">DateTimeOffset</span></span>|<span data-ttu-id="d07db-116">证书过期时间</span><span class="sxs-lookup"><span data-stu-id="d07db-116">Certificate expire time</span></span>|
|<span data-ttu-id="d07db-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="d07db-117">enrollmentError</span></span>|<span data-ttu-id="d07db-118">String</span><span class="sxs-lookup"><span data-stu-id="d07db-118">String</span></span>|<span data-ttu-id="d07db-119">证书连接器注册错误</span><span class="sxs-lookup"><span data-stu-id="d07db-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="d07db-120">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="d07db-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="d07db-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d07db-121">DateTimeOffset</span></span>|<span data-ttu-id="d07db-122">上次连接证书连接器的时间</span><span class="sxs-lookup"><span data-stu-id="d07db-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="d07db-123">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="d07db-123">connectorVersion</span></span>|<span data-ttu-id="d07db-124">String</span><span class="sxs-lookup"><span data-stu-id="d07db-124">String</span></span>|<span data-ttu-id="d07db-125">证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="d07db-125">Version of certificate connector</span></span>|
|<span data-ttu-id="d07db-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="d07db-126">lastUploadVersion</span></span>|<span data-ttu-id="d07db-127">Int64</span><span class="sxs-lookup"><span data-stu-id="d07db-127">Int64</span></span>|<span data-ttu-id="d07db-128">上次上载的证书连接器的版本</span><span class="sxs-lookup"><span data-stu-id="d07db-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="d07db-129">关系</span><span class="sxs-lookup"><span data-stu-id="d07db-129">Relationships</span></span>
<span data-ttu-id="d07db-130">无</span><span class="sxs-lookup"><span data-stu-id="d07db-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d07db-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d07db-131">JSON Representation</span></span>
<span data-ttu-id="d07db-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d07db-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```





