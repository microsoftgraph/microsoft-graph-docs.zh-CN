---
title: educationIdentityCreationConfiguration 资源类型
description: 创建学校数据配置文件标识上定义的设置。 这些身份包括学生和教师。 根据这些设置，将在目录中创建用户。
localization_priority: Normal
ms.openlocfilehash: 86624c7203dc6425372556572c40efda2bc1a53f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858861"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="bf41f-105">educationIdentityCreationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf41f-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="bf41f-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf41f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf41f-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf41f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf41f-108">创建学校数据配置文件标识上定义的设置。</span><span class="sxs-lookup"><span data-stu-id="bf41f-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="bf41f-109">这些身份包括学生和教师。</span><span class="sxs-lookup"><span data-stu-id="bf41f-109">These identities include students and teachers.</span></span> <span data-ttu-id="bf41f-110">根据这些设置，将在目录中创建用户。</span><span class="sxs-lookup"><span data-stu-id="bf41f-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="bf41f-111">**注意：** 如果您有目录同步到本地之间的同步开启，Active Directory 和 Azure Active Directory (Azure AD)，请改用[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)资源。</span><span class="sxs-lookup"><span data-stu-id="bf41f-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="bf41f-112">派生自[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bf41f-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bf41f-113">属性</span><span class="sxs-lookup"><span data-stu-id="bf41f-113">Properties</span></span>

| <span data-ttu-id="bf41f-114">属性</span><span class="sxs-lookup"><span data-stu-id="bf41f-114">Property</span></span> | <span data-ttu-id="bf41f-115">类型</span><span class="sxs-lookup"><span data-stu-id="bf41f-115">Type</span></span> | <span data-ttu-id="bf41f-116">Description</span><span class="sxs-lookup"><span data-stu-id="bf41f-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bf41f-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="bf41f-117">**userDomains**</span></span> | <span data-ttu-id="bf41f-118">[educationIdentityDomain](educationidentitydomain.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf41f-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="bf41f-119">设置要使用的每个用户类型的域的列表。</span><span class="sxs-lookup"><span data-stu-id="bf41f-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="bf41f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf41f-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
