---
title: iosSingleSignOnSettings 资源类型
description: iOS 的单一登录的 Kerberos 身份验证设置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421317"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="756b1-103">iosSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="756b1-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="756b1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="756b1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="756b1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="756b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="756b1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="756b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="756b1-107">iOS 的单一登录的 Kerberos 身份验证设置</span><span class="sxs-lookup"><span data-stu-id="756b1-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="756b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="756b1-108">Properties</span></span>
|<span data-ttu-id="756b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="756b1-109">Property</span></span>|<span data-ttu-id="756b1-110">类型</span><span class="sxs-lookup"><span data-stu-id="756b1-110">Type</span></span>|<span data-ttu-id="756b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="756b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="756b1-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="756b1-112">allowedAppsList</span></span>|<span data-ttu-id="756b1-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="756b1-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="756b1-114">允许使用此登录名的应用程序标识符的列表。</span><span class="sxs-lookup"><span data-stu-id="756b1-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="756b1-115">如果省略此字段，则在登录适用于设备上的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="756b1-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="756b1-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="756b1-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="756b1-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="756b1-117">allowedUrls</span></span>|<span data-ttu-id="756b1-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="756b1-118">String collection</span></span>|<span data-ttu-id="756b1-119">必须匹配才能使用此登录名的 HTTP Url 的列表。</span><span class="sxs-lookup"><span data-stu-id="756b1-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="756b1-120">与 iOS 9.0 或更高版本中，可以使用通配符。</span><span class="sxs-lookup"><span data-stu-id="756b1-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="756b1-121">displayName</span><span class="sxs-lookup"><span data-stu-id="756b1-121">displayName</span></span>|<span data-ttu-id="756b1-122">String</span><span class="sxs-lookup"><span data-stu-id="756b1-122">String</span></span>|<span data-ttu-id="756b1-123">接收设备上显示的登录设置显示名称。</span><span class="sxs-lookup"><span data-stu-id="756b1-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="756b1-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="756b1-124">kerberosPrincipalName</span></span>|<span data-ttu-id="756b1-125">String</span><span class="sxs-lookup"><span data-stu-id="756b1-125">String</span></span>|<span data-ttu-id="756b1-126">Kerberos 的主体名称。</span><span class="sxs-lookup"><span data-stu-id="756b1-126">A Kerberos principal name.</span></span> <span data-ttu-id="756b1-127">如果未提供，一个配置文件安装过程中提示用户。</span><span class="sxs-lookup"><span data-stu-id="756b1-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="756b1-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="756b1-128">kerberosRealm</span></span>|<span data-ttu-id="756b1-129">String</span><span class="sxs-lookup"><span data-stu-id="756b1-129">String</span></span>|<span data-ttu-id="756b1-130">Kerberos 领域名。</span><span class="sxs-lookup"><span data-stu-id="756b1-130">A Kerberos realm name.</span></span> <span data-ttu-id="756b1-131">区分大小写。</span><span class="sxs-lookup"><span data-stu-id="756b1-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="756b1-132">关系</span><span class="sxs-lookup"><span data-stu-id="756b1-132">Relationships</span></span>
<span data-ttu-id="756b1-133">无</span><span class="sxs-lookup"><span data-stu-id="756b1-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="756b1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="756b1-134">JSON Representation</span></span>
<span data-ttu-id="756b1-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="756b1-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```




