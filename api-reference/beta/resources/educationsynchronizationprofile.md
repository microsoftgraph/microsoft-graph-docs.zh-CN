---
title: educationSynchronizationProfile 资源类型
description: 表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。 此资源提供在学校数据同步中使用的编程表示形式。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 05babeebb25130350e64d98ccfc408381547829e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790913"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="7d91b-104">educationSynchronizationProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d91b-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="7d91b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d91b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d91b-106">表示一组用于将源目录中的教育实体和名单信息同步到 Azure Active Directory （Azure AD）的配置。</span><span class="sxs-lookup"><span data-stu-id="7d91b-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="7d91b-107">此资源提供在[学校数据同步](https://sds.microsoft.com)中使用的编程表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d91b-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="7d91b-108">Methods</span><span class="sxs-lookup"><span data-stu-id="7d91b-108">Methods</span></span>

| <span data-ttu-id="7d91b-109">方法</span><span class="sxs-lookup"><span data-stu-id="7d91b-109">Method</span></span>                                                                    | <span data-ttu-id="7d91b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d91b-110">Return Type</span></span>                                                 | <span data-ttu-id="7d91b-111">说明</span><span class="sxs-lookup"><span data-stu-id="7d91b-111">Description</span></span>                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="7d91b-112">列出配置文件</span><span class="sxs-lookup"><span data-stu-id="7d91b-112">List profiles</span></span>](../api/educationsynchronizationprofile-list.md)           | <span data-ttu-id="7d91b-113">[educationSynchronizationProfile]集合</span><span class="sxs-lookup"><span data-stu-id="7d91b-113">[educationSynchronizationProfile] collection</span></span>                | <span data-ttu-id="7d91b-114">获取租户中所有同步配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="7d91b-114">Get a list of all the synchronization profiles in the tenant.</span></span>                                                                  |
| [<span data-ttu-id="7d91b-115">获取个人资料</span><span class="sxs-lookup"><span data-stu-id="7d91b-115">Get profile</span></span>](../api/educationsynchronizationprofile-get.md)              | <span data-ttu-id="7d91b-116">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="7d91b-116">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="7d91b-117">在给定配置文件标识符的情况检索特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="7d91b-117">Retrieve a specific profile given the profile identifier.</span></span>                                                                      |
| [<span data-ttu-id="7d91b-118">创建配置文件</span><span class="sxs-lookup"><span data-stu-id="7d91b-118">Create profile</span></span>](../api/educationsynchronizationprofile-post.md)          | <span data-ttu-id="7d91b-119">无</span><span class="sxs-lookup"><span data-stu-id="7d91b-119">None</span></span>                                                        | <span data-ttu-id="7d91b-120">创建新的同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="7d91b-120">Create a new synchronization profile.</span></span>                                                                                          |
| [<span data-ttu-id="7d91b-121">删除个人资料</span><span class="sxs-lookup"><span data-stu-id="7d91b-121">Delete profile</span></span>](../api/educationsynchronizationprofile-delete.md)        | <span data-ttu-id="7d91b-122">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="7d91b-122">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="7d91b-123">在给定配置文件标识符的情况删除特定配置文件。</span><span class="sxs-lookup"><span data-stu-id="7d91b-123">Delete a specific profile given the profile identifier.</span></span>                                                                        |
| [<span data-ttu-id="7d91b-124">暂停配置文件</span><span class="sxs-lookup"><span data-stu-id="7d91b-124">Pause profile</span></span>](../api/educationsynchronizationprofile-pause.md)          | <span data-ttu-id="7d91b-125">无</span><span class="sxs-lookup"><span data-stu-id="7d91b-125">None</span></span>                                                        | <span data-ttu-id="7d91b-126">暂停正在进行的同步。</span><span class="sxs-lookup"><span data-stu-id="7d91b-126">Pause an ongoing synchronization.</span></span>                                                                                              |
| [<span data-ttu-id="7d91b-127">恢复配置文件</span><span class="sxs-lookup"><span data-stu-id="7d91b-127">Resume profile</span></span>](../api/educationsynchronizationprofile-resume.md)        | <span data-ttu-id="7d91b-128">无</span><span class="sxs-lookup"><span data-stu-id="7d91b-128">None</span></span>                                                        | <span data-ttu-id="7d91b-129">恢复暂停的同步。</span><span class="sxs-lookup"><span data-stu-id="7d91b-129">Resume a paused synchronization.</span></span>                                                                                               |
| [<span data-ttu-id="7d91b-130">重置配置文件</span><span class="sxs-lookup"><span data-stu-id="7d91b-130">Reset profile</span></span>](../api/educationsynchronizationprofile-reset.md)          | <span data-ttu-id="7d91b-131">无</span><span class="sxs-lookup"><span data-stu-id="7d91b-131">None</span></span>                                                        | <span data-ttu-id="7d91b-132">重置配置文件的状态并重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="7d91b-132">Reset the state of the profile and restart synchronization.</span></span>                                                                    |
| [<span data-ttu-id="7d91b-133">启动 CSV 配置文件</span><span class="sxs-lookup"><span data-stu-id="7d91b-133">Start CSV profile</span></span>](../api/educationsynchronizationprofile-start.md)      | <span data-ttu-id="7d91b-134">[educationFileSynchronizationVerificationMessage]集合</span><span class="sxs-lookup"><span data-stu-id="7d91b-134">[educationFileSynchronizationVerificationMessage]collection</span></span> | <span data-ttu-id="7d91b-135">验证上载的源文件并启动同步。</span><span class="sxs-lookup"><span data-stu-id="7d91b-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="7d91b-136">仅在数据提供程序为[educationCsvDataProvider]时适用。</span><span class="sxs-lookup"><span data-stu-id="7d91b-136">Applies only when the data provider is [educationCsvDataProvider].</span></span> |
| [<span data-ttu-id="7d91b-137">获取 CSV 上载 URL</span><span class="sxs-lookup"><span data-stu-id="7d91b-137">Get CSV upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="7d91b-138">string</span><span class="sxs-lookup"><span data-stu-id="7d91b-138">string</span></span>                                                      | <span data-ttu-id="7d91b-139">返回短生存期的 URL 以上载 CSV 数据文件。</span><span class="sxs-lookup"><span data-stu-id="7d91b-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="7d91b-140">仅在数据提供程序为[educationCsvDataProvider]时适用。</span><span class="sxs-lookup"><span data-stu-id="7d91b-140">Applies only when the data provider is [educationCsvDataProvider].</span></span>        |
| [<span data-ttu-id="7d91b-141">获取状态</span><span class="sxs-lookup"><span data-stu-id="7d91b-141">Get status</span></span>](../api/educationsynchronizationprofilestatus-get.md)         | <span data-ttu-id="7d91b-142">[educationsynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="7d91b-142">[educationsynchronizationProfileStatus]</span></span>                     | <span data-ttu-id="7d91b-143">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="7d91b-143">Return the status of a specific synchronization profile.</span></span>                                                                       |
| [<span data-ttu-id="7d91b-144">获取错误</span><span class="sxs-lookup"><span data-stu-id="7d91b-144">Get errors</span></span>](../api/educationsynchronizationerrors-get.md)                | <span data-ttu-id="7d91b-145">[educationSynchronizationError]集合</span><span class="sxs-lookup"><span data-stu-id="7d91b-145">[educationSynchronizationError] collection</span></span>                  | <span data-ttu-id="7d91b-146">获取同步过程中生成的所有错误。</span><span class="sxs-lookup"><span data-stu-id="7d91b-146">Get all the errors generated during synchronization.</span></span>                                                                           |

## <a name="properties"></a><span data-ttu-id="7d91b-147">属性</span><span class="sxs-lookup"><span data-stu-id="7d91b-147">Properties</span></span>

| <span data-ttu-id="7d91b-148">属性</span><span class="sxs-lookup"><span data-stu-id="7d91b-148">Property</span></span>                             | <span data-ttu-id="7d91b-149">类型</span><span class="sxs-lookup"><span data-stu-id="7d91b-149">Type</span></span>                                                   | <span data-ttu-id="7d91b-150">说明</span><span class="sxs-lookup"><span data-stu-id="7d91b-150">Description</span></span>                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7d91b-151">displayName</span><span class="sxs-lookup"><span data-stu-id="7d91b-151">displayName</span></span>                          | <span data-ttu-id="7d91b-152">string</span><span class="sxs-lookup"><span data-stu-id="7d91b-152">string</span></span>                                                 | <span data-ttu-id="7d91b-153">用于同步标识的配置文件的名称。</span><span class="sxs-lookup"><span data-stu-id="7d91b-153">Name of the configuration profile for syncing identities.</span></span>                                                                         |
| <span data-ttu-id="7d91b-154">dataProvider</span><span class="sxs-lookup"><span data-stu-id="7d91b-154">dataProvider</span></span>                         | <span data-ttu-id="7d91b-155">[educationSynchronizationDataProvider]</span><span class="sxs-lookup"><span data-stu-id="7d91b-155">[educationSynchronizationDataProvider]</span></span>                 | <span data-ttu-id="7d91b-156">用于配置文件的数据提供程序。</span><span class="sxs-lookup"><span data-stu-id="7d91b-156">The data provider used for the profile.</span></span>                                                                                           |
| <span data-ttu-id="7d91b-157">identitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d91b-157">identitySynchronizationConfiguration</span></span> | <span data-ttu-id="7d91b-158">[educationIdentitySynchronizationConfiguration]</span><span class="sxs-lookup"><span data-stu-id="7d91b-158">[educationIdentitySynchronizationConfiguration]</span></span>        | <span data-ttu-id="7d91b-159">确定配置文件应如何[新建][fullsync]或[匹配现有][dirsync]AAD 用户。</span><span class="sxs-lookup"><span data-stu-id="7d91b-159">Determines how the Profile should [create new][fullsync] or [match existing][dirsync] AAD Users.</span></span>                                  |
| <span data-ttu-id="7d91b-160">licensesToAssign</span><span class="sxs-lookup"><span data-stu-id="7d91b-160">licensesToAssign</span></span>                     | <span data-ttu-id="7d91b-161">[educationSynchronizationLicenseAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="7d91b-161">[educationSynchronizationLicenseAssignment] collection</span></span> | <span data-ttu-id="7d91b-162">许可证安装程序配置。</span><span class="sxs-lookup"><span data-stu-id="7d91b-162">License setup configuration.</span></span>                                                                                                      |
| <span data-ttu-id="7d91b-163">state</span><span class="sxs-lookup"><span data-stu-id="7d91b-163">state</span></span>                                | <span data-ttu-id="7d91b-164">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="7d91b-164">educationSynchronizationProfileState</span></span>                   | <span data-ttu-id="7d91b-165">配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="7d91b-165">The state of the profile.</span></span> <span data-ttu-id="7d91b-166">可取值为：`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed`。</span><span class="sxs-lookup"><span data-stu-id="7d91b-166">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7d91b-167">关系</span><span class="sxs-lookup"><span data-stu-id="7d91b-167">Relationships</span></span>

| <span data-ttu-id="7d91b-168">关系</span><span class="sxs-lookup"><span data-stu-id="7d91b-168">Relationship</span></span>  | <span data-ttu-id="7d91b-169">类型</span><span class="sxs-lookup"><span data-stu-id="7d91b-169">Type</span></span>                                       | <span data-ttu-id="7d91b-170">说明</span><span class="sxs-lookup"><span data-stu-id="7d91b-170">Description</span></span>                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| <span data-ttu-id="7d91b-171">错误</span><span class="sxs-lookup"><span data-stu-id="7d91b-171">errors</span></span>        | <span data-ttu-id="7d91b-172">[educationSynchronizationError]集合</span><span class="sxs-lookup"><span data-stu-id="7d91b-172">[educationSynchronizationError] collection</span></span> | <span data-ttu-id="7d91b-173">与此同步配置文件关联的所有错误。</span><span class="sxs-lookup"><span data-stu-id="7d91b-173">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="7d91b-174">profileStatus</span><span class="sxs-lookup"><span data-stu-id="7d91b-174">profileStatus</span></span> | <span data-ttu-id="7d91b-175">[educationSynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="7d91b-175">[educationSynchronizationProfileStatus]</span></span>    | <span data-ttu-id="7d91b-176">同步状态。</span><span class="sxs-lookup"><span data-stu-id="7d91b-176">The synchronization status.</span></span>                              |

## <a name="data-providers"></a><span data-ttu-id="7d91b-177">数据提供程序</span><span class="sxs-lookup"><span data-stu-id="7d91b-177">Data Providers</span></span>

<span data-ttu-id="7d91b-178">每个[educationSynchronizationProfile]必须指定要用作同步源的以下数据提供程序之一。</span><span class="sxs-lookup"><span data-stu-id="7d91b-178">Each [educationSynchronizationProfile] must specify one of the follow data providers to use as the synchronization source.</span></span>

| <span data-ttu-id="7d91b-179">Data Provider</span><span class="sxs-lookup"><span data-stu-id="7d91b-179">Data Provider</span></span>                       | <span data-ttu-id="7d91b-180">说明</span><span class="sxs-lookup"><span data-stu-id="7d91b-180">Description</span></span>                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7d91b-181">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="7d91b-181">[educationCsvDataProvider]</span></span>          | <span data-ttu-id="7d91b-182">上载到配置文件的[SAS URL](../api/educationsynchronizationprofile-uploadurl.md)的 CSV 文件</span><span class="sxs-lookup"><span data-stu-id="7d91b-182">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="7d91b-183">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="7d91b-183">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="7d91b-184">OneRoster v1.1 API</span><span class="sxs-lookup"><span data-stu-id="7d91b-184">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="7d91b-185">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="7d91b-185">[educationPowerSchoolDataProvider]</span></span>  | <span data-ttu-id="7d91b-186">PowerSchool API</span><span class="sxs-lookup"><span data-stu-id="7d91b-186">PowerSchool API</span></span>                                                                                    |

## <a name="json-representation"></a><span data-ttu-id="7d91b-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d91b-187">JSON representation</span></span>

<span data-ttu-id="7d91b-188">下面是**educationSynchronizationProfile**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d91b-188">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "state": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileState"
  },
  "profileStatus": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
  },
  "errors": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
    }
  ],
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationCsvDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "handleSpecialCharacterConstraint": "Boolean"
}
```

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationsynchronizationprofilestatus]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[educationfilesynchronizationverificationmessage]: educationFileSynchronizationVerificationMessage.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationidentitysynchronizationconfiguration]: educationIdentitySynchronizationConfiguration.md
[educationsynchronizationlicenseassignment]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationSynchronizationProfile/dataProvider:\r\n      Referenced type microsoft.graph.educationSynchronizationDataProvider is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
