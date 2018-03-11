---
swagger: "2.0"
info:
  title: Google Service Management
  description: Google Service Management allows service producers to publish their
    services on Google Cloud Platform so that they can be discovered and used by service
    consumers.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: servicemanagement.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: Sets the access control policy on the specified resource
      operationId: servicemanagement.services.setIamPolicy
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - iam
definitions:
  Advice:
    properties:
      description:
        description: This is a default description.
        type: post
  Api:
    properties:
      methods:
        description: This is a default description.
        type: post
      mixins:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      options:
        description: This is a default description.
        type: post
      syntax:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  AuditConfig:
    properties:
      auditLogConfigs:
        description: This is a default description.
        type: post
      exemptedMembers:
        description: This is a default description.
        type: post
      service:
        description: This is a default description.
        type: post
  AuditLogConfig:
    properties:
      exemptedMembers:
        description: This is a default description.
        type: post
      logType:
        description: This is a default description.
        type: post
  AuthProvider:
    properties:
      audiences:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      issuer:
        description: This is a default description.
        type: post
      jwksUri:
        description: This is a default description.
        type: post
  AuthRequirement:
    properties:
      audiences:
        description: This is a default description.
        type: post
      providerId:
        description: This is a default description.
        type: post
  Authentication:
    properties:
      providers:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
  AuthenticationRule:
    properties:
      allowWithoutCredential:
        description: This is a default description.
        type: post
      requirements:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  AuthorizationConfig:
    properties:
      provider:
        description: This is a default description.
        type: post
  Backend:
    properties:
      rules:
        description: This is a default description.
        type: post
  BackendRule:
    properties:
      address:
        description: This is a default description.
        type: post
      deadline:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  Binding:
    properties:
      members:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  ChangeReport:
    properties:
      configChanges:
        description: This is a default description.
        type: post
  CloudAuditOptions:
    properties: []
  Condition:
    properties:
      iam:
        description: This is a default description.
        type: post
      op:
        description: This is a default description.
        type: post
      svc:
        description: This is a default description.
        type: post
      sys:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
      values:
        description: This is a default description.
        type: post
  ConfigChange:
    properties:
      advices:
        description: This is a default description.
        type: post
      changeType:
        description: This is a default description.
        type: post
      element:
        description: This is a default description.
        type: post
      newValue:
        description: This is a default description.
        type: post
      oldValue:
        description: This is a default description.
        type: post
  ConfigFile:
    properties:
      fileContents:
        description: This is a default description.
        type: post
      filePath:
        description: This is a default description.
        type: post
      fileType:
        description: This is a default description.
        type: post
  ConfigRef:
    properties:
      name:
        description: This is a default description.
        type: post
  ConfigSource:
    properties:
      files:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
  Context:
    properties:
      rules:
        description: This is a default description.
        type: post
  ContextRule:
    properties:
      provided:
        description: This is a default description.
        type: post
      requested:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  Control:
    properties:
      environment:
        description: This is a default description.
        type: post
  CounterOptions:
    properties:
      field:
        description: This is a default description.
        type: post
      metric:
        description: This is a default description.
        type: post
  CustomError:
    properties:
      rules:
        description: This is a default description.
        type: post
      types:
        description: This is a default description.
        type: post
  CustomErrorRule:
    properties:
      isErrorType:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  CustomHttpPattern:
    properties:
      kind:
        description: This is a default description.
        type: post
      path:
        description: This is a default description.
        type: post
  DataAccessOptions:
    properties: []
  DeleteServiceStrategy:
    properties: []
  Diagnostic:
    properties:
      kind:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  DisableServiceRequest:
    properties:
      consumerId:
        description: This is a default description.
        type: post
  Documentation:
    properties:
      documentationRootUrl:
        description: This is a default description.
        type: post
      overview:
        description: This is a default description.
        type: post
      pages:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
      summary:
        description: This is a default description.
        type: post
  DocumentationRule:
    properties:
      deprecationDescription:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  EnableServiceRequest:
    properties:
      consumerId:
        description: This is a default description.
        type: post
  Endpoint:
    properties:
      aliases:
        description: This is a default description.
        type: post
      allowCors:
        description: This is a default description.
        type: post
      apis:
        description: This is a default description.
        type: post
      features:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  Enum:
    properties:
      enumvalue:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      options:
        description: This is a default description.
        type: post
      syntax:
        description: This is a default description.
        type: post
  EnumValue:
    properties:
      name:
        description: This is a default description.
        type: post
      number:
        description: This is a default description.
        type: post
      options:
        description: This is a default description.
        type: post
  Experimental:
    properties: []
  Field:
    properties:
      cardinality:
        description: This is a default description.
        type: post
      defaultValue:
        description: This is a default description.
        type: post
      jsonName:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      number:
        description: This is a default description.
        type: post
      oneofIndex:
        description: This is a default description.
        type: post
      options:
        description: This is a default description.
        type: post
      packed:
        description: This is a default description.
        type: post
      typeUrl:
        description: This is a default description.
        type: post
  GenerateConfigReportRequest:
    properties:
      newConfig:
        description: This is a default description.
        type: post
      oldConfig:
        description: This is a default description.
        type: post
  GenerateConfigReportResponse:
    properties:
      changeReports:
        description: This is a default description.
        type: post
      diagnostics:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      serviceName:
        description: This is a default description.
        type: post
  GetIamPolicyRequest:
    properties: []
  Http:
    properties:
      rules:
        description: This is a default description.
        type: post
  HttpRule:
    properties:
      additionalBindings:
        description: This is a default description.
        type: post
      body:
        description: This is a default description.
        type: post
      delete:
        description: This is a default description.
        type: post
      get:
        description: This is a default description.
        type: post
      patch:
        description: This is a default description.
        type: post
      post:
        description: This is a default description.
        type: post
      put:
        description: This is a default description.
        type: post
      responseBody:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  LabelDescriptor:
    properties:
      description:
        description: This is a default description.
        type: post
      key:
        description: This is a default description.
        type: post
      valueType:
        description: This is a default description.
        type: post
  ListOperationsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      operations:
        description: This is a default description.
        type: post
  ListServiceConfigsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      serviceConfigs:
        description: This is a default description.
        type: post
  ListServiceRolloutsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      rollouts:
        description: This is a default description.
        type: post
  ListServicesResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      services:
        description: This is a default description.
        type: post
  LogConfig:
    properties: []
  LogDescriptor:
    properties:
      description:
        description: This is a default description.
        type: post
      displayName:
        description: This is a default description.
        type: post
      labels:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  Logging:
    properties:
      consumerDestinations:
        description: This is a default description.
        type: post
      producerDestinations:
        description: This is a default description.
        type: post
  LoggingDestination:
    properties:
      logs:
        description: This is a default description.
        type: post
      monitoredResource:
        description: This is a default description.
        type: post
  ManagedService:
    properties:
      producerProjectId:
        description: This is a default description.
        type: post
      serviceName:
        description: This is a default description.
        type: post
  MediaDownload:
    properties:
      downloadService:
        description: This is a default description.
        type: post
      enabled:
        description: This is a default description.
        type: post
  MediaUpload:
    properties:
      enabled:
        description: This is a default description.
        type: post
      uploadService:
        description: This is a default description.
        type: post
  Method:
    properties:
      name:
        description: This is a default description.
        type: post
      options:
        description: This is a default description.
        type: post
      requestStreaming:
        description: This is a default description.
        type: post
      requestTypeUrl:
        description: This is a default description.
        type: post
      responseStreaming:
        description: This is a default description.
        type: post
      responseTypeUrl:
        description: This is a default description.
        type: post
      syntax:
        description: This is a default description.
        type: post
  MetricDescriptor:
    properties:
      description:
        description: This is a default description.
        type: post
      displayName:
        description: This is a default description.
        type: post
      labels:
        description: This is a default description.
        type: post
      metricKind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      unit:
        description: This is a default description.
        type: post
      valueType:
        description: This is a default description.
        type: post
  Mixin:
    properties:
      name:
        description: This is a default description.
        type: post
      root:
        description: This is a default description.
        type: post
  MonitoredResourceDescriptor:
    properties:
      description:
        description: This is a default description.
        type: post
      displayName:
        description: This is a default description.
        type: post
      labels:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  Monitoring:
    properties:
      consumerDestinations:
        description: This is a default description.
        type: post
      producerDestinations:
        description: This is a default description.
        type: post
  MonitoringDestination:
    properties:
      metrics:
        description: This is a default description.
        type: post
      monitoredResource:
        description: This is a default description.
        type: post
  OAuthRequirements:
    properties:
      canonicalScopes:
        description: This is a default description.
        type: post
  Operation:
    properties:
      done:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      response:
        description: This is a default description.
        type: post
  OperationMetadata:
    properties:
      progressPercentage:
        description: This is a default description.
        type: post
      resourceNames:
        description: This is a default description.
        type: post
      startTime:
        description: This is a default description.
        type: post
      steps:
        description: This is a default description.
        type: post
  Option:
    properties:
      name:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  Page:
    properties:
      content:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      subpages:
        description: This is a default description.
        type: post
  Policy:
    properties:
      auditConfigs:
        description: This is a default description.
        type: post
      bindings:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      iamOwned:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  Rollout:
    properties:
      createTime:
        description: This is a default description.
        type: post
      createdBy:
        description: This is a default description.
        type: post
      rolloutId:
        description: This is a default description.
        type: post
      serviceName:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
  Rule:
    properties:
      action:
        description: This is a default description.
        type: post
      conditions:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      in:
        description: This is a default description.
        type: post
      logConfig:
        description: This is a default description.
        type: post
      notIn:
        description: This is a default description.
        type: post
      permissions:
        description: This is a default description.
        type: post
  Service:
    properties:
      apis:
        description: This is a default description.
        type: post
      configVersion:
        description: This is a default description.
        type: post
      endpoints:
        description: This is a default description.
        type: post
      enums:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      logs:
        description: This is a default description.
        type: post
      metrics:
        description: This is a default description.
        type: post
      monitoredResources:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      producerProjectId:
        description: This is a default description.
        type: post
  SetIamPolicyRequest:
    properties:
      updateMask:
        description: This is a default description.
        type: post
  SourceContext:
    properties:
      fileName:
        description: This is a default description.
        type: post
  SourceInfo:
    properties:
      sourceFiles:
        description: This is a default description.
        type: post
  Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  Step:
    properties:
      description:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
  SubmitConfigSourceRequest:
    properties:
      validateOnly:
        description: This is a default description.
        type: post
  SubmitConfigSourceResponse:
    properties: []
  SystemParameter:
    properties:
      httpHeader:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      urlQueryParameter:
        description: This is a default description.
        type: post
  SystemParameterRule:
    properties:
      parameters:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  SystemParameters:
    properties:
      rules:
        description: This is a default description.
        type: post
  TestIamPermissionsRequest:
    properties:
      permissions:
        description: This is a default description.
        type: post
  TestIamPermissionsResponse:
    properties:
      permissions:
        description: This is a default description.
        type: post
  TrafficPercentStrategy:
    properties:
      percentages:
        description: This is a default description.
        type: post
  Type:
    properties:
      fields:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      oneofs:
        description: This is a default description.
        type: post
      options:
        description: This is a default description.
        type: post
      syntax:
        description: This is a default description.
        type: post
  UndeleteServiceResponse:
    properties: []
  Usage:
    properties:
      producerNotificationChannel:
        description: This is a default description.
        type: post
      requirements:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
  UsageRule:
    properties:
      allowUnregisteredCalls:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
  Visibility:
    properties:
      rules:
        description: This is a default description.
        type: post
  VisibilityRule:
    properties:
      restriction:
        description: This is a default description.
        type: post
      selector:
        description: This is a default description.
        type: post
x-collection-name: Google Service Management
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---