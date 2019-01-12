---
title: androidDeviceOwnerEnrollmentProfile 资源类型
description: 注册配置文件，用于使用 Google 的云管理注册 COSU 设备。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 5e609f16978f3dd68eb680692149954f83e6cc6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963554"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a><span data-ttu-id="5cf67-103">androidDeviceOwnerEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cf67-103">androidDeviceOwnerEnrollmentProfile resource type</span></span>

> <span data-ttu-id="5cf67-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5cf67-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cf67-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5cf67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cf67-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5cf67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cf67-107">注册配置文件，用于使用 Google 的云管理注册 COSU 设备。</span><span class="sxs-lookup"><span data-stu-id="5cf67-107">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>
## <a name="methods"></a><span data-ttu-id="5cf67-108">方法</span><span class="sxs-lookup"><span data-stu-id="5cf67-108">Methods</span></span>
|<span data-ttu-id="5cf67-109">方法</span><span class="sxs-lookup"><span data-stu-id="5cf67-109">Method</span></span>|<span data-ttu-id="5cf67-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5cf67-110">Return Type</span></span>|<span data-ttu-id="5cf67-111">说明</span><span class="sxs-lookup"><span data-stu-id="5cf67-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5cf67-112">列表 androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="5cf67-112">List androidDeviceOwnerEnrollmentProfiles</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|<span data-ttu-id="5cf67-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cf67-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) collection</span></span>|<span data-ttu-id="5cf67-114">列出属性和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="5cf67-114">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="5cf67-115">获取 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5cf67-115">Get androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[<span data-ttu-id="5cf67-116">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5cf67-116">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="5cf67-117">读取属性和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5cf67-117">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5cf67-118">创建 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5cf67-118">Create androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[<span data-ttu-id="5cf67-119">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5cf67-119">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="5cf67-120">创建新的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5cf67-120">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5cf67-121">删除 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5cf67-121">Delete androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|<span data-ttu-id="5cf67-122">无</span><span class="sxs-lookup"><span data-stu-id="5cf67-122">None</span></span>|<span data-ttu-id="5cf67-123">删除[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="5cf67-123">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="5cf67-124">更新 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5cf67-124">Update androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[<span data-ttu-id="5cf67-125">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5cf67-125">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="5cf67-126">更新[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5cf67-126">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5cf67-127">revokeToken 操作</span><span class="sxs-lookup"><span data-stu-id="5cf67-127">revokeToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|<span data-ttu-id="5cf67-128">无</span><span class="sxs-lookup"><span data-stu-id="5cf67-128">None</span></span>|<span data-ttu-id="5cf67-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cf67-129">Not yet documented</span></span>|
|[<span data-ttu-id="5cf67-130">createToken 操作</span><span class="sxs-lookup"><span data-stu-id="5cf67-130">createToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|<span data-ttu-id="5cf67-131">无</span><span class="sxs-lookup"><span data-stu-id="5cf67-131">None</span></span>|<span data-ttu-id="5cf67-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5cf67-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5cf67-133">属性</span><span class="sxs-lookup"><span data-stu-id="5cf67-133">Properties</span></span>
|<span data-ttu-id="5cf67-134">属性</span><span class="sxs-lookup"><span data-stu-id="5cf67-134">Property</span></span>|<span data-ttu-id="5cf67-135">类型</span><span class="sxs-lookup"><span data-stu-id="5cf67-135">Type</span></span>|<span data-ttu-id="5cf67-136">说明</span><span class="sxs-lookup"><span data-stu-id="5cf67-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cf67-137">accountId</span><span class="sxs-lookup"><span data-stu-id="5cf67-137">accountId</span></span>|<span data-ttu-id="5cf67-138">String</span><span class="sxs-lookup"><span data-stu-id="5cf67-138">String</span></span>|<span data-ttu-id="5cf67-139">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="5cf67-139">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="5cf67-140">id</span><span class="sxs-lookup"><span data-stu-id="5cf67-140">id</span></span>|<span data-ttu-id="5cf67-141">String</span><span class="sxs-lookup"><span data-stu-id="5cf67-141">String</span></span>|<span data-ttu-id="5cf67-142">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="5cf67-142">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="5cf67-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5cf67-143">displayName</span></span>|<span data-ttu-id="5cf67-144">String</span><span class="sxs-lookup"><span data-stu-id="5cf67-144">String</span></span>|<span data-ttu-id="5cf67-145">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5cf67-145">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="5cf67-146">description</span><span class="sxs-lookup"><span data-stu-id="5cf67-146">description</span></span>|<span data-ttu-id="5cf67-147">String</span><span class="sxs-lookup"><span data-stu-id="5cf67-147">String</span></span>|<span data-ttu-id="5cf67-148">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="5cf67-148">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="5cf67-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf67-149">createdDateTime</span></span>|<span data-ttu-id="5cf67-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf67-150">DateTimeOffset</span></span>|<span data-ttu-id="5cf67-151">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5cf67-151">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="5cf67-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf67-152">lastModifiedDateTime</span></span>|<span data-ttu-id="5cf67-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf67-153">DateTimeOffset</span></span>|<span data-ttu-id="5cf67-154">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5cf67-154">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="5cf67-155">tokenValue</span><span class="sxs-lookup"><span data-stu-id="5cf67-155">tokenValue</span></span>|<span data-ttu-id="5cf67-156">String</span><span class="sxs-lookup"><span data-stu-id="5cf67-156">String</span></span>|<span data-ttu-id="5cf67-157">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="5cf67-157">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="5cf67-158">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf67-158">tokenCreationDateTime</span></span>|<span data-ttu-id="5cf67-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf67-159">DateTimeOffset</span></span>|<span data-ttu-id="5cf67-160">创建日期时间最近创建的令牌。</span><span class="sxs-lookup"><span data-stu-id="5cf67-160">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="5cf67-161">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf67-161">tokenExpirationDateTime</span></span>|<span data-ttu-id="5cf67-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf67-162">DateTimeOffset</span></span>|<span data-ttu-id="5cf67-163">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5cf67-163">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="5cf67-164">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5cf67-164">enrolledDeviceCount</span></span>|<span data-ttu-id="5cf67-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5cf67-165">Int32</span></span>|<span data-ttu-id="5cf67-166">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="5cf67-166">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="5cf67-167">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="5cf67-167">qrCodeContent</span></span>|<span data-ttu-id="5cf67-168">String</span><span class="sxs-lookup"><span data-stu-id="5cf67-168">String</span></span>|<span data-ttu-id="5cf67-169">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="5cf67-169">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="5cf67-170">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="5cf67-170">qrCodeImage</span></span>|[<span data-ttu-id="5cf67-171">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5cf67-171">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5cf67-172">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="5cf67-172">String used to generate a QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cf67-173">关系</span><span class="sxs-lookup"><span data-stu-id="5cf67-173">Relationships</span></span>
<span data-ttu-id="5cf67-174">无</span><span class="sxs-lookup"><span data-stu-id="5cf67-174">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5cf67-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cf67-175">JSON Representation</span></span>
<span data-ttu-id="5cf67-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cf67-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```





