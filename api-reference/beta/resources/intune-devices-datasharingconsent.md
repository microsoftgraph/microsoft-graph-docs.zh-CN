---
title: dataSharingConsent 资源类型
description: 数据共享许可信息。
ms.openlocfilehash: 152b367161dc9a734a20e007ac1b2c0d02d0c99f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049252"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="6bf7e-103">dataSharingConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bf7e-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="6bf7e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bf7e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bf7e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf7e-107">数据共享许可信息。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-107">Data sharing consent information.</span></span>
## <a name="methods"></a><span data-ttu-id="6bf7e-108">方法</span><span class="sxs-lookup"><span data-stu-id="6bf7e-108">Methods</span></span>
|<span data-ttu-id="6bf7e-109">方法</span><span class="sxs-lookup"><span data-stu-id="6bf7e-109">Method</span></span>|<span data-ttu-id="6bf7e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6bf7e-110">Return Type</span></span>|<span data-ttu-id="6bf7e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6bf7e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bf7e-112">列表 dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="6bf7e-112">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="6bf7e-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bf7e-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="6bf7e-114">列出属性和[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-114">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="6bf7e-115">获取 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-115">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="6bf7e-116">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-116">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="6bf7e-117">读取属性和[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-117">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="6bf7e-118">创建 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-118">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="6bf7e-119">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-119">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="6bf7e-120">创建新的[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-120">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="6bf7e-121">删除 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-121">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="6bf7e-122">无</span><span class="sxs-lookup"><span data-stu-id="6bf7e-122">None</span></span>|<span data-ttu-id="6bf7e-123">删除[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-123">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="6bf7e-124">更新 dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-124">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="6bf7e-125">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-125">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="6bf7e-126">更新[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-126">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="6bf7e-127">consentToDataSharing 操作</span><span class="sxs-lookup"><span data-stu-id="6bf7e-127">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="6bf7e-128">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="6bf7e-128">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="6bf7e-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6bf7e-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6bf7e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6bf7e-130">Properties</span></span>
|<span data-ttu-id="6bf7e-131">属性</span><span class="sxs-lookup"><span data-stu-id="6bf7e-131">Property</span></span>|<span data-ttu-id="6bf7e-132">类型</span><span class="sxs-lookup"><span data-stu-id="6bf7e-132">Type</span></span>|<span data-ttu-id="6bf7e-133">说明</span><span class="sxs-lookup"><span data-stu-id="6bf7e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf7e-134">id</span><span class="sxs-lookup"><span data-stu-id="6bf7e-134">id</span></span>|<span data-ttu-id="6bf7e-135">字符串</span><span class="sxs-lookup"><span data-stu-id="6bf7e-135">String</span></span>|<span data-ttu-id="6bf7e-136">数据共享同意 Id</span><span class="sxs-lookup"><span data-stu-id="6bf7e-136">The data sharing consent Id</span></span>|
|<span data-ttu-id="6bf7e-137">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6bf7e-137">serviceDisplayName</span></span>|<span data-ttu-id="6bf7e-138">字符串</span><span class="sxs-lookup"><span data-stu-id="6bf7e-138">String</span></span>|<span data-ttu-id="6bf7e-139">服务工作流的显示名称</span><span class="sxs-lookup"><span data-stu-id="6bf7e-139">The display name of the service work flow</span></span>|
|<span data-ttu-id="6bf7e-140">termsUrl</span><span class="sxs-lookup"><span data-stu-id="6bf7e-140">termsUrl</span></span>|<span data-ttu-id="6bf7e-141">字符串</span><span class="sxs-lookup"><span data-stu-id="6bf7e-141">String</span></span>|<span data-ttu-id="6bf7e-142">数据共享同意 TermsUrl</span><span class="sxs-lookup"><span data-stu-id="6bf7e-142">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="6bf7e-143">授予</span><span class="sxs-lookup"><span data-stu-id="6bf7e-143">granted</span></span>|<span data-ttu-id="6bf7e-144">布尔</span><span class="sxs-lookup"><span data-stu-id="6bf7e-144">Boolean</span></span>|<span data-ttu-id="6bf7e-145">数据共享同意向其授予的状态</span><span class="sxs-lookup"><span data-stu-id="6bf7e-145">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="6bf7e-146">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="6bf7e-146">grantDateTime</span></span>|<span data-ttu-id="6bf7e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bf7e-147">DateTimeOffset</span></span>|<span data-ttu-id="6bf7e-148">此帐户授予时间同意</span><span class="sxs-lookup"><span data-stu-id="6bf7e-148">The time consent was granted for this account</span></span>|
|<span data-ttu-id="6bf7e-149">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="6bf7e-149">grantedByUpn</span></span>|<span data-ttu-id="6bf7e-150">字符串</span><span class="sxs-lookup"><span data-stu-id="6bf7e-150">String</span></span>|<span data-ttu-id="6bf7e-151">用户授予许可，为此帐户的 Upn</span><span class="sxs-lookup"><span data-stu-id="6bf7e-151">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="6bf7e-152">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="6bf7e-152">grantedByUserId</span></span>|<span data-ttu-id="6bf7e-153">字符串</span><span class="sxs-lookup"><span data-stu-id="6bf7e-153">String</span></span>|<span data-ttu-id="6bf7e-154">授予许可，为此帐户的用户的用户 Id</span><span class="sxs-lookup"><span data-stu-id="6bf7e-154">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bf7e-155">Relationships</span><span class="sxs-lookup"><span data-stu-id="6bf7e-155">Relationships</span></span>
<span data-ttu-id="6bf7e-156">无</span><span class="sxs-lookup"><span data-stu-id="6bf7e-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6bf7e-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bf7e-157">JSON Representation</span></span>
<span data-ttu-id="6bf7e-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bf7e-158">Here is a JSON representation of the resource.</span></span>
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





