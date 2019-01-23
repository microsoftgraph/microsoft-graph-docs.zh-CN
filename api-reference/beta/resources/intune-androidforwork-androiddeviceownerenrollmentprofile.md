---
title: androidDeviceOwnerEnrollmentProfile 资源类型
description: 注册配置文件，用于使用 Google 的云管理注册 COSU 设备。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 931360e917eab8e8fbddadf70b70aafb39f7c50b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416662"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a><span data-ttu-id="86250-103">androidDeviceOwnerEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="86250-103">androidDeviceOwnerEnrollmentProfile resource type</span></span>

> <span data-ttu-id="86250-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="86250-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86250-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86250-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86250-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86250-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86250-107">注册配置文件，用于使用 Google 的云管理注册 COSU 设备。</span><span class="sxs-lookup"><span data-stu-id="86250-107">Enrollment Profile used to enroll COSU devices using Google's Cloud Management.</span></span>

## <a name="methods"></a><span data-ttu-id="86250-108">方法</span><span class="sxs-lookup"><span data-stu-id="86250-108">Methods</span></span>
|<span data-ttu-id="86250-109">方法</span><span class="sxs-lookup"><span data-stu-id="86250-109">Method</span></span>|<span data-ttu-id="86250-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="86250-110">Return Type</span></span>|<span data-ttu-id="86250-111">说明</span><span class="sxs-lookup"><span data-stu-id="86250-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86250-112">列表 androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="86250-112">List androidDeviceOwnerEnrollmentProfiles</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|<span data-ttu-id="86250-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="86250-113">[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) collection</span></span>|<span data-ttu-id="86250-114">列出属性和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="86250-114">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="86250-115">获取 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86250-115">Get androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[<span data-ttu-id="86250-116">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86250-116">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="86250-117">读取属性和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="86250-117">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="86250-118">创建 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86250-118">Create androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[<span data-ttu-id="86250-119">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86250-119">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="86250-120">创建新的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86250-120">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="86250-121">删除 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86250-121">Delete androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|<span data-ttu-id="86250-122">无</span><span class="sxs-lookup"><span data-stu-id="86250-122">None</span></span>|<span data-ttu-id="86250-123">删除[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="86250-123">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="86250-124">更新 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86250-124">Update androidDeviceOwnerEnrollmentProfile</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[<span data-ttu-id="86250-125">androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86250-125">androidDeviceOwnerEnrollmentProfile</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|<span data-ttu-id="86250-126">更新[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86250-126">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="86250-127">revokeToken 操作</span><span class="sxs-lookup"><span data-stu-id="86250-127">revokeToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|<span data-ttu-id="86250-128">无</span><span class="sxs-lookup"><span data-stu-id="86250-128">None</span></span>|<span data-ttu-id="86250-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="86250-129">Not yet documented</span></span>|
|[<span data-ttu-id="86250-130">createToken 操作</span><span class="sxs-lookup"><span data-stu-id="86250-130">createToken action</span></span>](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|<span data-ttu-id="86250-131">无</span><span class="sxs-lookup"><span data-stu-id="86250-131">None</span></span>|<span data-ttu-id="86250-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="86250-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="86250-133">属性</span><span class="sxs-lookup"><span data-stu-id="86250-133">Properties</span></span>
|<span data-ttu-id="86250-134">属性</span><span class="sxs-lookup"><span data-stu-id="86250-134">Property</span></span>|<span data-ttu-id="86250-135">类型</span><span class="sxs-lookup"><span data-stu-id="86250-135">Type</span></span>|<span data-ttu-id="86250-136">说明</span><span class="sxs-lookup"><span data-stu-id="86250-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86250-137">accountId</span><span class="sxs-lookup"><span data-stu-id="86250-137">accountId</span></span>|<span data-ttu-id="86250-138">String</span><span class="sxs-lookup"><span data-stu-id="86250-138">String</span></span>|<span data-ttu-id="86250-139">注册配置文件所属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="86250-139">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="86250-140">id</span><span class="sxs-lookup"><span data-stu-id="86250-140">id</span></span>|<span data-ttu-id="86250-141">String</span><span class="sxs-lookup"><span data-stu-id="86250-141">String</span></span>|<span data-ttu-id="86250-142">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="86250-142">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="86250-143">displayName</span><span class="sxs-lookup"><span data-stu-id="86250-143">displayName</span></span>|<span data-ttu-id="86250-144">String</span><span class="sxs-lookup"><span data-stu-id="86250-144">String</span></span>|<span data-ttu-id="86250-145">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="86250-145">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="86250-146">description</span><span class="sxs-lookup"><span data-stu-id="86250-146">description</span></span>|<span data-ttu-id="86250-147">String</span><span class="sxs-lookup"><span data-stu-id="86250-147">String</span></span>|<span data-ttu-id="86250-148">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="86250-148">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="86250-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86250-149">createdDateTime</span></span>|<span data-ttu-id="86250-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86250-150">DateTimeOffset</span></span>|<span data-ttu-id="86250-151">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86250-151">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="86250-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86250-152">lastModifiedDateTime</span></span>|<span data-ttu-id="86250-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86250-153">DateTimeOffset</span></span>|<span data-ttu-id="86250-154">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86250-154">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="86250-155">tokenValue</span><span class="sxs-lookup"><span data-stu-id="86250-155">tokenValue</span></span>|<span data-ttu-id="86250-156">String</span><span class="sxs-lookup"><span data-stu-id="86250-156">String</span></span>|<span data-ttu-id="86250-157">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="86250-157">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="86250-158">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="86250-158">tokenCreationDateTime</span></span>|<span data-ttu-id="86250-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86250-159">DateTimeOffset</span></span>|<span data-ttu-id="86250-160">创建日期时间最近创建的令牌。</span><span class="sxs-lookup"><span data-stu-id="86250-160">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="86250-161">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="86250-161">tokenExpirationDateTime</span></span>|<span data-ttu-id="86250-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86250-162">DateTimeOffset</span></span>|<span data-ttu-id="86250-163">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86250-163">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="86250-164">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86250-164">enrolledDeviceCount</span></span>|<span data-ttu-id="86250-165">Int32</span><span class="sxs-lookup"><span data-stu-id="86250-165">Int32</span></span>|<span data-ttu-id="86250-166">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="86250-166">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="86250-167">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="86250-167">qrCodeContent</span></span>|<span data-ttu-id="86250-168">String</span><span class="sxs-lookup"><span data-stu-id="86250-168">String</span></span>|<span data-ttu-id="86250-169">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="86250-169">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="86250-170">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="86250-170">qrCodeImage</span></span>|[<span data-ttu-id="86250-171">mimeContent</span><span class="sxs-lookup"><span data-stu-id="86250-171">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="86250-172">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="86250-172">String used to generate a QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86250-173">关系</span><span class="sxs-lookup"><span data-stu-id="86250-173">Relationships</span></span>
<span data-ttu-id="86250-174">无</span><span class="sxs-lookup"><span data-stu-id="86250-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86250-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86250-175">JSON Representation</span></span>
<span data-ttu-id="86250-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86250-176">Here is a JSON representation of the resource.</span></span>
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




