---
title: deviceManagementDerivedCredentialSettings 资源类型
description: 描述派生凭据的租户级别设置的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2b9d81cf542681bc2ef610ebe86e836d7c84412
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332776"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="76c66-103">deviceManagementDerivedCredentialSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="76c66-103">deviceManagementDerivedCredentialSettings resource type</span></span>

> <span data-ttu-id="76c66-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76c66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76c66-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76c66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76c66-106">描述派生凭据的租户级别设置的实体</span><span class="sxs-lookup"><span data-stu-id="76c66-106">Entity that describes tenant level settings for derived credentials</span></span>

## <a name="methods"></a><span data-ttu-id="76c66-107">方法</span><span class="sxs-lookup"><span data-stu-id="76c66-107">Methods</span></span>
|<span data-ttu-id="76c66-108">方法</span><span class="sxs-lookup"><span data-stu-id="76c66-108">Method</span></span>|<span data-ttu-id="76c66-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="76c66-109">Return Type</span></span>|<span data-ttu-id="76c66-110">说明</span><span class="sxs-lookup"><span data-stu-id="76c66-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76c66-111">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="76c66-111">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="76c66-112">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="76c66-112">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="76c66-113">读取[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76c66-113">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="76c66-114">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="76c66-114">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="76c66-115">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="76c66-115">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="76c66-116">更新[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="76c66-116">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="76c66-117">属性</span><span class="sxs-lookup"><span data-stu-id="76c66-117">Properties</span></span>
|<span data-ttu-id="76c66-118">属性</span><span class="sxs-lookup"><span data-stu-id="76c66-118">Property</span></span>|<span data-ttu-id="76c66-119">类型</span><span class="sxs-lookup"><span data-stu-id="76c66-119">Type</span></span>|<span data-ttu-id="76c66-120">说明</span><span class="sxs-lookup"><span data-stu-id="76c66-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76c66-121">id</span><span class="sxs-lookup"><span data-stu-id="76c66-121">id</span></span>|<span data-ttu-id="76c66-122">String</span><span class="sxs-lookup"><span data-stu-id="76c66-122">String</span></span>|<span data-ttu-id="76c66-123">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="76c66-123">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="76c66-124">helpUrl</span><span class="sxs-lookup"><span data-stu-id="76c66-124">helpUrl</span></span>|<span data-ttu-id="76c66-125">String</span><span class="sxs-lookup"><span data-stu-id="76c66-125">String</span></span>|<span data-ttu-id="76c66-126">最终用户在使用公司门户检索派生凭据时将可访问的 URL。</span><span class="sxs-lookup"><span data-stu-id="76c66-126">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="76c66-127">displayName</span><span class="sxs-lookup"><span data-stu-id="76c66-127">displayName</span></span>|<span data-ttu-id="76c66-128">String</span><span class="sxs-lookup"><span data-stu-id="76c66-128">String</span></span>|<span data-ttu-id="76c66-129">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="76c66-129">The display name for the profile.</span></span>|
|<span data-ttu-id="76c66-130">常用</span><span class="sxs-lookup"><span data-stu-id="76c66-130">issuer</span></span>|[<span data-ttu-id="76c66-131">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="76c66-131">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="76c66-132">要使用的派生凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="76c66-132">The derived credential provider to use.</span></span> <span data-ttu-id="76c66-133">可取值为：`intercede`、`entrustDatacard`、`purebred`。</span><span class="sxs-lookup"><span data-stu-id="76c66-133">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="76c66-134">notificationType</span><span class="sxs-lookup"><span data-stu-id="76c66-134">notificationType</span></span>|[<span data-ttu-id="76c66-135">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="76c66-135">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="76c66-136">用于通知最终用户打开公司门户以传递使用证书到设备的 Wi-fi、VPN 或电子邮件配置文件的方法。</span><span class="sxs-lookup"><span data-stu-id="76c66-136">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="76c66-137">可取值为：`none`、`companyPortal`、`email`。</span><span class="sxs-lookup"><span data-stu-id="76c66-137">Possible values are: `none`, `companyPortal`, `email`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76c66-138">关系</span><span class="sxs-lookup"><span data-stu-id="76c66-138">Relationships</span></span>
<span data-ttu-id="76c66-139">无</span><span class="sxs-lookup"><span data-stu-id="76c66-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76c66-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76c66-140">JSON Representation</span></span>
<span data-ttu-id="76c66-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76c66-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```



