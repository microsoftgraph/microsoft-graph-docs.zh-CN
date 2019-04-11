---
title: dataSharingConsent 资源类型
description: 数据共享同意信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e1cb144957ee000a4e077f0f9c58065fad3a8dc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780194"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="8b2d7-103">dataSharingConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b2d7-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="8b2d7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b2d7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b2d7-106">数据共享同意信息。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-106">Data sharing consent information.</span></span>

## <a name="methods"></a><span data-ttu-id="8b2d7-107">方法</span><span class="sxs-lookup"><span data-stu-id="8b2d7-107">Methods</span></span>
|<span data-ttu-id="8b2d7-108">方法</span><span class="sxs-lookup"><span data-stu-id="8b2d7-108">Method</span></span>|<span data-ttu-id="8b2d7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8b2d7-109">Return Type</span></span>|<span data-ttu-id="8b2d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="8b2d7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b2d7-111">列出 dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="8b2d7-111">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="8b2d7-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)集合</span><span class="sxs-lookup"><span data-stu-id="8b2d7-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="8b2d7-113">列出[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-113">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="8b2d7-114">获取 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-114">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="8b2d7-115">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-115">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="8b2d7-116">读取[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-116">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="8b2d7-117">创建 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-117">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="8b2d7-118">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-118">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="8b2d7-119">创建新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-119">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="8b2d7-120">删除 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-120">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="8b2d7-121">无</span><span class="sxs-lookup"><span data-stu-id="8b2d7-121">None</span></span>|<span data-ttu-id="8b2d7-122">删除[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-122">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="8b2d7-123">更新 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-123">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="8b2d7-124">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-124">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="8b2d7-125">更新[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-125">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="8b2d7-126">consentToDataSharing 操作</span><span class="sxs-lookup"><span data-stu-id="8b2d7-126">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="8b2d7-127">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="8b2d7-127">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="8b2d7-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8b2d7-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8b2d7-129">属性</span><span class="sxs-lookup"><span data-stu-id="8b2d7-129">Properties</span></span>
|<span data-ttu-id="8b2d7-130">属性</span><span class="sxs-lookup"><span data-stu-id="8b2d7-130">Property</span></span>|<span data-ttu-id="8b2d7-131">类型</span><span class="sxs-lookup"><span data-stu-id="8b2d7-131">Type</span></span>|<span data-ttu-id="8b2d7-132">说明</span><span class="sxs-lookup"><span data-stu-id="8b2d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b2d7-133">id</span><span class="sxs-lookup"><span data-stu-id="8b2d7-133">id</span></span>|<span data-ttu-id="8b2d7-134">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-134">String</span></span>|<span data-ttu-id="8b2d7-135">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="8b2d7-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="8b2d7-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8b2d7-136">serviceDisplayName</span></span>|<span data-ttu-id="8b2d7-137">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-137">String</span></span>|<span data-ttu-id="8b2d7-138">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="8b2d7-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="8b2d7-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="8b2d7-139">termsUrl</span></span>|<span data-ttu-id="8b2d7-140">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-140">String</span></span>|<span data-ttu-id="8b2d7-141">数据共享同意的 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="8b2d7-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="8b2d7-142">granted</span><span class="sxs-lookup"><span data-stu-id="8b2d7-142">granted</span></span>|<span data-ttu-id="8b2d7-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="8b2d7-143">Boolean</span></span>|<span data-ttu-id="8b2d7-144">"数据共享同意" 的 "已授予" 状态</span><span class="sxs-lookup"><span data-stu-id="8b2d7-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="8b2d7-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="8b2d7-145">grantDateTime</span></span>|<span data-ttu-id="8b2d7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b2d7-146">DateTimeOffset</span></span>|<span data-ttu-id="8b2d7-147">授予此帐户的时间许可</span><span class="sxs-lookup"><span data-stu-id="8b2d7-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="8b2d7-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="8b2d7-148">grantedByUpn</span></span>|<span data-ttu-id="8b2d7-149">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-149">String</span></span>|<span data-ttu-id="8b2d7-150">授予此帐户同意的用户的 Upn</span><span class="sxs-lookup"><span data-stu-id="8b2d7-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="8b2d7-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="8b2d7-151">grantedByUserId</span></span>|<span data-ttu-id="8b2d7-152">String</span><span class="sxs-lookup"><span data-stu-id="8b2d7-152">String</span></span>|<span data-ttu-id="8b2d7-153">授予此帐户同意的用户的用户 id</span><span class="sxs-lookup"><span data-stu-id="8b2d7-153">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b2d7-154">关系</span><span class="sxs-lookup"><span data-stu-id="8b2d7-154">Relationships</span></span>
<span data-ttu-id="8b2d7-155">无</span><span class="sxs-lookup"><span data-stu-id="8b2d7-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b2d7-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b2d7-156">JSON Representation</span></span>
<span data-ttu-id="8b2d7-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b2d7-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```





